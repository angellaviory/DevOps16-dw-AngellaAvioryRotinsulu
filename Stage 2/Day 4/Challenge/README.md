## Buatlah BASH Script untuk Instalasi Docker 
1. Buat file nano docker.sh

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


## Buatlah Dockerized Image Sekecil mungkin (Frontend)
1. Masuk ke directory literature-frontend dan tambahkan tag **alpine** pada versi node di Dockerfile
<img width="572" alt="Screenshot 2023-04-16 at 13 34 29" src="https://user-images.githubusercontent.com/102456153/232277192-467fe168-0195-478c-9f8c-8dda249bc973.png">

2. Kemudian build aplikasi literature-frontend versi alphine. Dapat dilihat, saya telah berhasil meng-dockerized image literature-frontend.
<img width="1237" alt="Screenshot 2023-04-16 at 13 19 42" src="https://user-images.githubusercontent.com/102456153/232277333-a8b41d80-78a4-4af7-9bc1-2a114c1c6e33.png">


## Jalankan NGINX On Top Docker
