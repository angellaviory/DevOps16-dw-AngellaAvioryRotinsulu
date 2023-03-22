# Web Server
### 1. Buat VM Tambahan untuk NGINX.
- Buka terminal komputer, kemudian buat instance multipass baru 
<img width="576" alt="Screenshot 2023-03-22 at 22 20 23" src="https://user-images.githubusercontent.com/102456153/226953416-5ac56f3b-7782-48f0-9795-202511695b9f.png">


- Jalankan instance baru dan mulai menginstall nginx
<img width="578" alt="Screenshot 2023-03-22 at 22 22 44" src="https://user-images.githubusercontent.com/102456153/226953430-f8422a63-b746-4e47-b369-bcc2163fe036.png">


- Nginx telah terinstall
<img width="1321" alt="Screenshot 2023-03-22 at 22 23 29" src="https://user-images.githubusercontent.com/102456153/226953515-aa5f6295-c301-4103-aa38-e846d86103e4.png">


### 2. Jalankan Aplikasi Dumbflix di PM2.
- Masuk ke dalam directory dumbflix
<img width="574" alt="Screenshot 2023-03-22 at 22 30 24" src="https://user-images.githubusercontent.com/102456153/226955917-fea9d228-1ea0-4fa0-8ccf-164c420bacfb.png">


- Jalankan aplikasi dumbflix di PM2
<img width="577" alt="Screenshot 2023-03-22 at 22 30 33" src="https://user-images.githubusercontent.com/102456153/226955933-0fe8b2b6-d9ca-4f56-82b0-7ff4f69885a3.png">


- Aplikasi dumbflix telah berhasil di jalankan 
<img width="1316" alt="Screenshot 2023-03-22 at 22 31 12" src="https://user-images.githubusercontent.com/102456153/226955955-217eef34-9c7f-4a1d-890d-002b1ff36ff2.png">


### 3. Buatlah Reverse Proxy dengan Directory /etc/nginx/dumbways.
- Pertama masuk ke dalam folder nginx


- Kemudian buat directory baru dengan nama "Dumbways"


- Setelah itu masuk ke dalam directory dumbways dan membuat file reverse proxy


- Dalam file tersebut, masukkan nama domain yang diinginkan dan IP lokal beserta port 3000


- Selanjutnya tambahkan konfigurasi baru pada file nginx.conf


- Pastikan tidak ada masalah dalam konfigurasi


- Jalankan Nginx


- Berikutnya membuat virtual host, dimana memasukkan IP dan domain yang sudah dibuat tadi


### 4. Dengan Nginx, Pastikan Dumbflix Bisa Diakses dengan Domain yang Diinginkan.

- Mencoba jalankan aplikasi dumbflix dengan menggunakan domain yang telah dibuat.



