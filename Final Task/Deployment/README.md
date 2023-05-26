# fe-dumbmerch
- Hal pertama saya lakukan adalah mengclone aplikasi dari repository github.
<img width="579" alt="Screenshot 2023-05-19 at 03 14 32" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/83450932-d901-4253-ac22-ee1969c7ab1e">

- Selanjutnya saya akan membuat file **.env** (environment), dimana saya akan memasukkan IP sehingga aplikasi dapat diakses.
```
REACT_APP_BASEURL=http://api.angel.studentdumbways.my.id/api/v1
```

- Kemudian saya akan membuat **Dockerfile** untuk mem-build image dumbmerch-frontend.
```
#staging
ROM node:16.16-alpine AS staging
WORKDIR /app
COPY . .
RUN npm install
EXPOSE 3000
CMD ["npm","start"]

#production
ROM node:16.16-alpine AS staging
WORKDIR /app
COPY . .
RUN npm install

FROM staging
WORKDIR /app
COPY --from=staging /app /app
EXPOSE 3000
CMD ["npm","start"]
```
- Saya akan mem-build Dockerfile tersbut. 
<img width="680" alt="Screenshot 2023-05-21 at 17 11 11" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/cb2c48e0-3a14-4dde-b239-6bc1717cbe09">

- Berikut menggunakan branch production.
<img width="561" alt="Screenshot 2023-05-27 at 00 44 00" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/9fb1ca85-23a3-4299-8a92-4a31cf67531d">



# be-dumbmerch
- Hal pertama saya lakukan adalah mengclone aplikasi dari repository github.
<img width="579" alt="Screenshot 2023-05-19 at 03 14 32" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/c8b5dffd-905b-4de9-b844-6eb6bb21cbfd">

- Selanjutnya saya akan membuat file **.env** (environment), dimana saya akan memasukkan IP sehingga aplikasi dapat diakses.
```
DB_HOST=10.52.49.248
DB_USER=ang
DB_PASSWORD=Dumbways1
DB_NAME=dumbmerch
DB_PORT=5423
PORT=5000
```
- Kemudian saya akan membuat **Dockerfile** untuk mem-build image dumbmerch-backend
```
#stagiing dan production
FROM golang:1.16
WORKDIR /app
COPY . .
RUN go get ./ && go build && go mod download
EXPOSE 5000
CMD ["go", "run", "main.go"]
```
- Saya akan mem-build Dockerfile tersbut. 
<img width="633" alt="Screenshot 2023-05-21 at 22 48 37" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/3335139d-3cf8-428c-bc0a-d906e63693c8">
<img width="563" alt="Screenshot 2023-05-27 at 00 47 24" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/0bce5030-2517-4303-a4ed-fbf1ebd0e6d4">

# Deployment
- Saya telah membuat image docker untuk dumbmerch-frontend dan dumbmerch-backend. Sekarang saya sudah bisa meng-compose aplikasi dumbmerch. Berikut script docker-compose.yml:
```
version: "3.8"
services:
  db:
    image: postgres:latest
    container_name: postgres
    ports:
      - 5432:5432
    volumes:
      - ~/postgresql:/var/lib/postgresql/data
    environment:
      - POSTGRES_USER=ang
      - POSTGRES_PASSWORD=dumbways1
      - POSTGRES_DB=dumbmerch

  be:
    depends_on:
      - db
    image: angellaviory/dumbmerchbe-production:latest
    container_name: be-dumbmerch
    stdin_open: true
    restart: unless-stopped
    ports:
      - 5000:5000

  fe:
    image: angellaviory/dumbmerchfe-production:latest
    container_name: fe-dumbmerch
    stdin_open: true
    restart: unless-stopped
    ports:
      - 3000:3000
```
<img width="608" alt="Screenshot 2023-05-27 at 00 51 14" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/3223a1f1-ecfa-4833-ba1c-07fe39b71cfb">

- Sekarang saya akan mencoba mengakses aplikasi Dumbmerch menggunakan browser. Saya telah berhasil mengakses aplikasi Dumbmerch.
<img width="1323" alt="Screenshot 2023-05-22 at 13 25 56" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2e5d3be6-02d5-4eaa-8bde-2e4701ec8be9">
<img width="1319" alt="Screenshot 2023-05-22 at 13 35 30" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/9341d09f-2ac7-4a29-ae1b-d445c2ba91ca">
<img width="1323" alt="Screenshot 2023-05-22 at 13 36 06" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/0f75eebc-8285-4f87-90c2-1308d5369d9a">

# CI/CD: Jenkins
- Agar bisa mengakses jenkins, pertama-tama masukkan password untuk meng-unlock jenkins.

- Kemudian saya memilih menginstall dengan menambah plugin tambahan, yaitu **ssh agent**. Setelah itu jenkins akan mulai mendownload.

- Sekarang saya akan meng-create user untuk jenkins.

- Setelah itu saya memasukkan IP public saya.

- Jenkins telah berhasil di install dan siap digunakan.

- Hal selanjutnya yang saya lakukan adalah membuat **cridentials** dan memasukkan **private-key** local ke jenkins. 

- Sekarang saya sudah bisa memulai membuat project. 

- Kemudian memasukkan repository github yang akan di automasi oleh jenkins.

- Berikut script file **Jenkinsfile**:
```
#frontend
def branch = "cicd"
def repo = "git@github.com:angellaviory/fe-dumbmerch.git"
def cred = "ang"
def dir = "~/fe-dumbmerch"
def server = "ang@103.31.38.155"
def imagename = "dumbmerch-fe"

pipeline {
    agent any
    stages {
        stage('Repository pull') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
		    mkdir ${dir}
                    cd ${dir}
		    git init
                    git remote add origin ${repo}
		    git pull origin master
		    git branch ${branch}
		    git checkout ${branch}
		    git pull origin ${branch}
                    exit
                    EOF
                    """
                }
            }
        }
    
        stage('Image Build') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    mkdir ${dir}
                    cd ${dir}
                    docker build -t ${imagename}:latest .
                    exit
                    EOF
                    """
                    }
               }
         }

         stage('Image Push') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    mkdir ${dir}
                    cd ${dir}
                    docker tag ${imagename}:latest angellaviory/dumbmerchfe-staging:latest
                    docker push angellaviory/dumbmerchfe-staging:latest
                    exit
                    EOF
                    """
                    }
               }
         }

         stage('Docker Run') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    mkdir ${dir}
                    cd ${dir}
                    docker run -d -p 3300:3000 ${imagename}:latest
                    exit
                    EOF
                    """
                    }
               }
         }

    }
}

#backend
def branch = "cicd"
def repo = "git@github.com:angellaviory/be-dumbmerch.git"
def cred = "ang"
def dir = "~/be-dumbmerch"
def server = "ang@103.31.38.155"
def imagename = "dumbmerch-be"

pipeline {
    agent any
    stages {
        stage('Repository pull') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
		    mkdir ${dir}
                    cd ${dir}
		    git init
                    git remote add origin ${repo}
		    git pull origin master
		    git branch ${branch}
		    git checkout ${branch}
		    git pull origin ${branch}
                    exit
                    EOF
                    """
                }
            }
        }
    
        stage('Image Build') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    mkdir ${dir}
                    cd ${dir}
                    docker build -t ${imagename}:latest .
                    exit
                    EOF
                    """
                    }
               }
         }

         stage('Image Push') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    mkdir ${dir}
                    cd ${dir}
                    docker tag ${imagename}:latest angellaviory/dumbmerchbe-staging:latest
                    docker push angellaviory/dumbmerchbe-staging:latest
                    exit
                    EOF
                    """
                    }
               }
         }

         stage('Docker Run') {
            steps {
                sshagent([cred]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    mkdir ${dir}
                    cd ${dir}
                    docker run -d -p 5500:5000 ${imagename}:latest
                    exit
                    EOF
                    """
                    }
               }
         }

    }
}
```

- Kemudian push file tersebut ke GitHub.

- Setelah itu, saya akan build project. Dapat dilihat, saya telah berhasil melakukan **Pull Repository**, **Build image**, **Push Image**, dan **Run Image**.
