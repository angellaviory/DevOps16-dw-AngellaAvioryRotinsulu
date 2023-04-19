## Buatlah BASH Script untuk Instalasi Docker 
1. Buat file nano docker.sh
<img width="811" alt="Screenshot 2023-04-19 at 17 32 39" src="https://user-images.githubusercontent.com/102456153/233049025-9c7e4cc2-3047-42ab-8488-23b7ee9e4e35.png">

2. Didalam file tersebut, tulis command untuk menginstall docker seperti dibawah ini.
```
#!/usr/bin/env bash

sudo apt-get update

sudo apt-get install
ca-certificates
curl
gnupg

sudo install -m 0755 -d/etc/apt/keyrings

curl -fsSL https://download.docker.com/linux/ubuntu/gpg sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

sudo chmod a+r /etc/apt/keyrings/docker.gpg

sudo aot-get undate

sudo apt-get install docker-ce docker-ce-cl1 contalnerd.10 docker-bulldx-plugin docker-compose-plugin
```

3. Kemudian jalankan perintah ``bash docker.sh`` dan docker pun akan terinstall
<img width="807" alt="Screenshot 2023-04-19 at 17 33 31" src="https://user-images.githubusercontent.com/102456153/233049063-000cdef8-cf36-4084-81ed-b1f0d2f8f86a.png">


## Buatlah Dockerized Image Sekecil mungkin (Frontend)
1. Masuk ke directory wayshub-frontend dan tambahkan tag **alpine** pada versi node di Dockerfile
<img width="572" alt="Screenshot 2023-04-19 at 17 01 44" src="https://user-images.githubusercontent.com/102456153/233047753-27432daf-9bef-4465-a9fb-3d2be7004f68.png">

2. Kemudian build aplikasi wayshub-frontend versi alphine. 
<img width="808" alt="Screenshot 2023-04-19 at 17 08 53" src="https://user-images.githubusercontent.com/102456153/233047764-68be848d-b0db-4ab8-87dd-27849dbfcada.png">

3. Wayshub-frontend telah berhasil di dockerized image dengan size kecil menggunakan alpine.
<img width="807" alt="Screenshot 2023-04-19 at 17 09 37" src="https://user-images.githubusercontent.com/102456153/233048133-1f645e3a-1f87-4484-a04b-b7247939341f.png">


4. Saya memasukkan ke DockerHub saya.
<img width="807" alt="Screenshot 2023-04-19 at 17 16 34" src="https://user-images.githubusercontent.com/102456153/233048173-325ac3ec-a420-4322-9981-f934824bdd22.png">
<img width="1347" alt="Screenshot 2023-04-19 at 17 24 52" src="https://user-images.githubusercontent.com/102456153/233048197-cae83282-00bb-45cd-bdac-160727ea1551.png">



## Jalankan NGINX On Top Docker
1. Pull nginx dari Docker Hub
<img width="767" alt="Screenshot 2023-04-17 at 03 49 29" src="https://user-images.githubusercontent.com/102456153/232341722-b4f971a5-edf1-47b1-a0ac-324cf52d66b4.png">

2. Memastikan bahwa nginx telah berhasil di pull
<img width="767" alt="Screenshot 2023-04-17 at 03 49 57" src="https://user-images.githubusercontent.com/102456153/232341726-8da96316-4bf4-4186-bbda-f86a574441ca.png">

3. Kemudian jalankan nginx
<img width="770" alt="Screenshot 2023-04-17 at 03 51 20" src="https://user-images.githubusercontent.com/102456153/232341731-9adf8d00-41d9-4ba8-afba-cde27bd57d0a.png">

4. Mengakses nginx di browser
<img width="1349" alt="Screenshot 2023-04-17 at 03 51 01" src="https://user-images.githubusercontent.com/102456153/232341734-6f49bee8-d861-44a6-9a76-a416722a5395.png">
