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
$ sudo apt install ufw -y
$ sudo ufw default deny incoming
$ sudo ufw default allow outgoing
$ sudo ufw allow 22
$ sudo ufw allow 80
$ sudo ufw allow 445
$ sudo ufw allow 3000 
$ sudo ufw status
$ sudo ufw enable
```
- `$ sudo apt install ufw -y`
> digunakan untuk menginstall firewall
<img width="575" alt="Screenshot 2023-03-20 at 22 48 39" src="https://user-images.githubusercontent.com/102456153/226414064-23deb027-8952-4fb4-95e9-fd0e8b10b827.png">


- `$ sudo ufw default deny incoming`
> digunakan untuk memblok akses dari luar ke dalam
<img width="576" alt="Screenshot 2023-03-20 at 22 49 10" src="https://user-images.githubusercontent.com/102456153/226414081-8802d731-a948-43bc-a6f9-b5bf28eb2700.png">


- `$ sudo ufw default allow outgoing`
> digunakan untuk memberikan akses dari dalam ke luar
<img width="577" alt="Screenshot 2023-03-20 at 22 49 21" src="https://user-images.githubusercontent.com/102456153/226414099-692c8a7e-7d54-4c5e-9872-ec8868aa855d.png">


- `$ sudo ufw allow 22`
> digunakan untuk memberikan akses SSH
<img width="575" alt="Screenshot 2023-03-20 at 22 50 24" src="https://user-images.githubusercontent.com/102456153/226413741-a5c1c257-06e2-4487-bff4-c0fea98e79e9.png">


- `$ sudo ufw allow 80`
> digunakan untuk memberikan akses HTTP
<img width="577" alt="Screenshot 2023-03-20 at 22 50 39" src="https://user-images.githubusercontent.com/102456153/226414143-4af89c27-c63c-4b39-b731-00a1858d6f6e.png">


- `$ sudo ufw allow 445`
> digunakan untuk memberikan akses HTTPS
<img width="574" alt="Screenshot 2023-03-20 at 22 50 50" src="https://user-images.githubusercontent.com/102456153/226414151-3383e637-1a22-4663-8565-5b40936ddd7c.png">


- `$ sudo ufw allow 3000 `
> digunakan untuk memberikan akses NODEJS
<img width="576" alt="Screenshot 2023-03-20 at 22 51 04" src="https://user-images.githubusercontent.com/102456153/226414164-a125f356-cba6-4255-b916-9e65f3ec031c.png">


- `$ sudo ufw status`
> digunakan untuk mengecek apa saja yang telah diberikan akses oleh firewall
<img width="574" alt="Screenshot 2023-03-20 at 22 54 34" src="https://user-images.githubusercontent.com/102456153/226414324-1141f94c-b268-4b33-beac-e1885cbbdf94.png">


- `$ sudo ufw enable`
> digunakan untuk menyalakan firewall
<img width="577" alt="Screenshot 2023-03-20 at 22 53 59" src="https://user-images.githubusercontent.com/102456153/226414339-02ce9cca-57b0-49ea-8de9-eb1240ae3513.png">



2. Update apt dan install Nginx
```
$ sudo apt update
$ sudo apt install nginx
```
- `$ sudo apt update`
<img width="574" alt="Screenshot 2023-03-20 at 15 36 29" src="https://user-images.githubusercontent.com/102456153/226287305-ee84a5bf-08b6-4840-b81d-d61f52ae6d0e.png">


- `$ sudo apt install nginx`
<img width="576" alt="Screenshot 2023-03-20 at 15 36 44" src="https://user-images.githubusercontent.com/102456153/226287313-52d45759-17a7-41d0-b84d-4ec0e245225d.png">


## Monitoring
### 1. Jelaskan tampilan HTOP

<img width="577" alt="Screenshot 2023-03-21 at 00 06 45" src="https://user-images.githubusercontent.com/102456153/226416680-b230de43-953a-4879-abbe-b9bc197a4dc6.png">

- CPU: CPU yang digunakan
- MEM: Total memory
- Swp: Memory pengganti
- Tasks: Memberitahukan aplikasi yang berjalan
- Load Averange: Rata-rata beban system yang berjalan
- Uptime: Menampilkan waktu berjalannya 
- PID: ID unik
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

