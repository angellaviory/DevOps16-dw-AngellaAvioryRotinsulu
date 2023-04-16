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
1. Pull nginx dari Docker Hub
<img width="767" alt="Screenshot 2023-04-17 at 03 49 29" src="https://user-images.githubusercontent.com/102456153/232341722-b4f971a5-edf1-47b1-a0ac-324cf52d66b4.png">

2. Memastikan bahwa nginx telah berhasil di pull
<img width="767" alt="Screenshot 2023-04-17 at 03 49 57" src="https://user-images.githubusercontent.com/102456153/232341726-8da96316-4bf4-4186-bbda-f86a574441ca.png">

3. Kemudian jalankan nginx
<img width="770" alt="Screenshot 2023-04-17 at 03 51 20" src="https://user-images.githubusercontent.com/102456153/232341731-9adf8d00-41d9-4ba8-afba-cde27bd57d0a.png">

4. Mengakses nginx di browser
<img width="1349" alt="Screenshot 2023-04-17 at 03 51 01" src="https://user-images.githubusercontent.com/102456153/232341734-6f49bee8-d861-44a6-9a76-a416722a5395.png">
