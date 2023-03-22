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
<img width="575" alt="Screenshot 2023-03-22 at 22 50 23" src="https://user-images.githubusercontent.com/102456153/226966495-93d68876-d151-402c-876c-7287fe5f5989.png">


- Kemudian buat directory baru dengan nama "Dumbways"
<img width="574" alt="Screenshot 2023-03-22 at 22 49 56" src="https://user-images.githubusercontent.com/102456153/226966506-0ede8c7a-0596-4fd4-9121-95f7e3c76bf9.png">


- Setelah itu masuk ke dalam directory dumbways dan membuat file reverse proxy. Dalam file tersebut, masukkan nama domain yang diinginkan dan IP lokal beserta port 3000
<img width="577" alt="Screenshot 2023-03-22 at 22 54 18" src="https://user-images.githubusercontent.com/102456153/226966824-07781910-988c-4480-aced-17bc0fc305e2.png">


- Selanjutnya tambahkan konfigurasi baru pada file nginx.conf
<img width="576" alt="Screenshot 2023-03-22 at 22 55 45" src="https://user-images.githubusercontent.com/102456153/226966842-a3230696-85e8-4db2-a462-852af207243a.png">


- Pastikan tidak ada masalah dalam konfigurasi
<img width="578" alt="Screenshot 2023-03-22 at 22 56 11" src="https://user-images.githubusercontent.com/102456153/226966867-99b191d6-20be-4b7a-a425-18eaeac2dee6.png">


- Restart Nginx agar konfigurasi tambahan dapat dijalankan
<img width="578" alt="Screenshot 2023-03-22 at 22 56 43" src="https://user-images.githubusercontent.com/102456153/226967111-4cc2e0ba-7dd1-407e-aafc-4f4ed3fefe69.png">


- Berikutnya membuat virtual host, dimana memasukkan IP dan domain yang sudah dibuat tadi di terminal komputer
<img width="576" alt="Screenshot 2023-03-22 at 22 57 55" src="https://user-images.githubusercontent.com/102456153/226967477-6b3ad402-25c6-4380-9f56-b0c8be03faf2.png">


### 4. Dengan Nginx, Pastikan Dumbflix Bisa Diakses dengan Domain yang Diinginkan.

- Masuk ke dalam directory dumbflix
<img width="575" alt="Screenshot 2023-03-22 at 22 59 19" src="https://user-images.githubusercontent.com/102456153/226966422-51e9fa69-3a2e-4f26-b23e-291955de1e20.png">


- Jalankan aplikasi dumbflix
<img width="575" alt="Screenshot 2023-03-22 at 22 59 45" src="https://user-images.githubusercontent.com/102456153/226966401-2e2c29f9-83ed-4e04-ac8d-2c01c7a5a1f3.png">


- Berhasil diakses menggunakan domain di browser
<img width="1327" alt="Screenshot 2023-03-22 at 23 00 14" src="https://user-images.githubusercontent.com/102456153/226966386-b3999e87-086b-4a80-9506-cf8a1c36cc04.png">





