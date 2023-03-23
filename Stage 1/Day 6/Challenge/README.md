# LOAD BALANCING
## Menggunakan 2 server, Jalankan Load Balancing yang berfungsi dengan baik
- Untuk mengecek load balancing berfungsi dengan baik, pertama kedua server harus memiliki aplikasi yang sama. Saya akan mengclone aplikasi dumbflix ke server kedua saya (**deevops**).
<img width="577" alt="Screenshot 2023-03-23 at 00 31 15" src="https://user-images.githubusercontent.com/102456153/227081796-67983a3d-16a3-4a96-9d49-b8d15e1f7e9d.png">


- Kemudian di server pertama(**devops**) masuk ke dalam directory nginx.
<img width="576" alt="Screenshot 2023-03-23 at 00 46 05" src="https://user-images.githubusercontent.com/102456153/227081806-c50651dc-8043-44a8-bda2-69728889d517.png">


- Berikutnya tambahkan upstream pada reverse proxy nginx.
<img width="577" alt="Screenshot 2023-03-23 at 00 49 10" src="https://user-images.githubusercontent.com/102456153/227081834-b37412ff-5b35-4d31-b3f6-210ae38e0396.png">


- Jangan lupa untuk menambahkan IP dan domain untuk server kedua di **/etc/hosts**.
<img width="571" alt="Screenshot 2023-03-23 at 00 56 15" src="https://user-images.githubusercontent.com/102456153/227081867-f9b6949c-2638-4f45-a416-00b6f5aa9c16.png">


- Aplikasi dumbflix telah berhasil dijalankan di server pertama menggunakan domain.
<img width="1325" alt="Screenshot 2023-03-23 at 00 53 16" src="https://user-images.githubusercontent.com/102456153/227081871-84081b7e-6f73-42a9-9ebe-1a5c70251ad9.png">


- Aplikasi dumbflix juga telah berhasil dijalankan di server kedua menggunakan domain.
<img width="1318" alt="Screenshot 2023-03-23 at 09 00 38" src="https://user-images.githubusercontent.com/102456153/227081876-38f60dce-b57b-4209-8a78-ee8554301fde.png">

