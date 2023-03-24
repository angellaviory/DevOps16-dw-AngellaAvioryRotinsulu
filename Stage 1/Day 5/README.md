# Manage Server in Terminal
## BASH
### 1. Jelaskan dan Contohkan Command untuk Text Manipulation!
**Text Manipulation** merupakan perintah teks yang dapat digunakan untuk memanipulasi file tanpa harus menggunakan text editor. Salah satu contoh dari text manipulation adalah **'Cat'** dimana command ini dapat digunakan untuk melihat isi dari sebuah file. Akan tetapi, dapat juga digunakan untuk menggabungkan dua file yang berbeda menjadi satu dan membuat file baru sekaligus memberikan isi pada file tersebut.
contoh: 
- Command *cat* untuk membuat file baru sekaligus memberikan isi pada file.
<img width="575" alt="Screenshot 2023-03-20 at 15 06 29" src="https://user-images.githubusercontent.com/102456153/226281761-aa600ebb-e3c5-41d1-bb92-51022a131c4f.png">

- Command *cat* untuk menggabungkan dua file menjadi satu.
<img width="576" alt="Screenshot 2023-03-20 at 15 08 27" src="https://user-images.githubusercontent.com/102456153/226281770-d962b364-3cd8-448d-89ac-4e397d8b0bf7.png">


### 2. Buatlah sebuah script untuk:
1. Memberikan akses ufw pada port 22, 80, 443 dan 3000.

```
sudo apt install ufw -y
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow 22
sudo ufw allow 80
sudo ufw allow 445
sudo ufw allow 3000 
sudo ufw status
sudo ufw enable
```
- Masuk ke dalam text editor **ufw.sh**
<img width="575" alt="Screenshot 2023-03-24 at 13 54 10" src="https://user-images.githubusercontent.com/102456153/227449400-68605569-4d79-40f4-bdc2-6b32fd2e0cf0.png">

- Copy dan paste script diatas dan save
<img width="577" alt="Screenshot 2023-03-24 at 13 55 36" src="https://user-images.githubusercontent.com/102456153/227449490-f54cf824-b5b5-4829-bbbd-88b00ecd5bc1.png">

- Jalankan bash ufw
<img width="578" alt="Screenshot 2023-03-24 at 14 03 41" src="https://user-images.githubusercontent.com/102456153/227449502-a7c5c417-c0f5-4d17-af4b-df582862ffcd.png">

## Monitoring
### 1. Jelaskan tampilan HTOP

<img width="577" alt="Screenshot 2023-03-21 at 00 06 45" src="https://user-images.githubusercontent.com/102456153/226416680-b230de43-953a-4879-abbe-b9bc197a4dc6.png">

- CPU: CPU yang digunakan
- MEM: Total memory
- Swp: Memory pengganti
- Tasks: Memberitahukan aplikasi yang berjalan
- Load Averange: Rata-rata beban system yang berjalan
- Uptime: Menampilkan waktu berjalannya 
- PID: ID 
- USER: pengguna/Owner 
- PRI: Prioritas dilihat dari linux karnel
- NI: Prioritas dilihat dari root atau user
- VIR: Virtual memory yang dipakai
- RES: Memory fisik yang dipakai
- SHR: Memory yang digunakan bersama
- S: Penggambaran keadaan sekarang
- CPU%: Persentase pemakaian CPU
- MEM%: Persentase pemakaian memory
- TIME+: Waktu berjalan dari semenjak diaktifkan
- Command: Nama command yang diproses


### 2. Gunakan NMON untuk menampilkan CPU, RAM Usage dan Network I/O!
> Saya ketik  c , m , n maka CPU RAM dan Network I/O akan muncul.
<img width="579" alt="Screenshot 2023-03-21 at 00 37 20" src="https://user-images.githubusercontent.com/102456153/226422725-b08d0db7-bdce-4bc9-bc20-bcc13d04c968.png">
<img width="575" alt="Screenshot 2023-03-21 at 00 39 05" src="https://user-images.githubusercontent.com/102456153/226422737-c86f104d-5b9b-45d7-ae31-c78949acc557.png">

