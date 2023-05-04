
# Buat 2 VM di IDCloudHost dengan spesifikasi berikut : 
Appserver : 1 CPU, 2 GB RAM
<img width="1008" alt="Screenshot 2023-04-06 at 14 33 43" src="https://user-images.githubusercontent.com/102456153/230782146-fa026425-3f06-466b-9c7d-85e9addacd55.png">

Gateway : 1 CPU, 2 GB RAM dan 20 GB Storage
<img width="1007" alt="Screenshot 2023-04-09 at 22 34 13" src="https://user-images.githubusercontent.com/102456153/230782139-d8bac4be-b611-4298-b00e-24419e605cef.png">

## 1. Deploy Wayshub
- Akses appserver melalui terminal dengan IP publik yang telah dibuat
<img width="569" alt="Screenshot 2023-04-06 at 14 36 48" src="https://user-images.githubusercontent.com/102456153/230804032-0bc511fd-d1ec-4e83-843b-aa7f831c177a.png">

- Update appserver terlebih dahulu
<img width="577" alt="Screenshot 2023-04-06 at 14 39 52" src="https://user-images.githubusercontent.com/102456153/230804034-15541c76-240a-4b3a-960a-317b5ea51452.png">

- Sebelum meng-clone, saya membuat directory baru untuk aplikasi wayshub
<img width="576" alt="Screenshot 2023-04-06 at 14 41 06" src="https://user-images.githubusercontent.com/102456153/230804039-f2158419-60d7-4870-b644-1a0fa9c26617.png">

- Kemudian saya meng-clone aplikasi wayshub baik frontend dan backend
<img width="576" alt="Screenshot 2023-04-06 at 14 41 43" src="https://user-images.githubusercontent.com/102456153/230804045-472a82f8-1fec-497e-90aa-a91cafba5ef3.png">
<img width="574" alt="Screenshot 2023-04-06 at 14 42 45" src="https://user-images.githubusercontent.com/102456153/230804051-6baa1d6e-bd2a-4b2a-bdca-a21bf8202bf1.png">

- Untuk dapat menajalankan aplikasi, dibutuhkan nvm sehingga harus menginstall nvm terlebih dahulu
<img width="572" alt="Screenshot 2023-04-06 at 14 47 13" src="https://user-images.githubusercontent.com/102456153/230804060-7a12916c-a110-43f8-bed6-036a6689c025.png">

- Setelah itu, saya menginstall nvm versi 14
<img width="574" alt="Screenshot 2023-04-06 at 14 50 11" src="https://user-images.githubusercontent.com/102456153/230804108-e9238c11-8a22-4f5e-adf5-f9e5fb53376d.png">

- Selanjutnya saya menginstall PM2
<img width="574" alt="Screenshot 2023-04-06 at 15 01 34" src="https://user-images.githubusercontent.com/102456153/230804143-1e83ee0a-034f-44d1-a1fc-1c39369a540c.png">

- Saya menggunakan PM2 untuk menjalankan aplikasi wayshub
<img width="578" alt="Screenshot 2023-04-06 at 15 17 14" src="https://user-images.githubusercontent.com/102456153/230804151-cc762735-9d44-4438-aac5-6cee0c64d76c.png">

- Berikut tampilan wayshub frontend dengan menggunakan IP Publik
<img width="1325" alt="Screenshot 2023-04-06 at 15 20 35" src="https://user-images.githubusercontent.com/102456153/230804154-9b791c77-e8f5-49bc-88e8-6dc9e8add5ab.png">

- Pada aplikasi wayshub, memiliki fitur **"Sign Up"**. Berarti data ini memerlukan tempat untuk penyimpanan data yang akan dikirimkan oleh backend. Tempat tersebut dinamankan *Database*. Berikut saya akan menginstall MYSQL Server yang merupakan salah satu bentuk database.
<img width="573" alt="Screenshot 2023-04-06 at 16 05 16" src="https://user-images.githubusercontent.com/102456153/230804201-e5d6e5a7-32e8-42f0-82c1-e09e1d3a3350.png">

- Saat pembuatan MYSQL, database root belum aman karena dapat diakses tanpa harus menggunakan password. Jadi saya akan menginstall ``mysql_secure`` agar database hanya dapat diakses menggunakan password 
<img width="578" alt="Screenshot 2023-04-06 at 16 48 03" src="https://user-images.githubusercontent.com/102456153/230804293-40f5862b-5d3e-4141-9b39-8f6542c2060e.png">


- Kembali ke directory wayshub backend, ganti configurasi BASEURL localhost:5000 di `api.js` dengan domain backend yang sudah dibuat
<img width="576" alt="Screenshot 2023-04-06 at 17 56 58" src="https://user-images.githubusercontent.com/102456153/230804484-9545c7c2-916e-4fe0-9c2e-893f89bbd9b5.png">
<img width="575" alt="Screenshot 2023-04-06 at 17 58 08" src="https://user-images.githubusercontent.com/102456153/230804497-6485c031-3f92-4e3b-901e-16657ff2d6a5.png">

- Kemudian masuk ke config.json untuk mengganti dibagian development username, password
<img width="577" alt="Screenshot 2023-04-06 at 17 59 46" src="https://user-images.githubusercontent.com/102456153/230804503-7df79563-200b-4954-b6a0-ddd4a787ea78.png">
<img width="572" alt="Screenshot 2023-04-07 at 15 25 21" src="https://user-images.githubusercontent.com/102456153/230804526-75ebafd4-43a3-4798-9ccb-f0206b6a230a.png">

- Install npm sequelize untuk menghubungkan backend dan database
<img width="575" alt="Screenshot 2023-04-07 at 15 19 43" src="https://user-images.githubusercontent.com/102456153/230804531-ac428e82-b5a8-49d3-b34a-8756b65b1c34.png">

- Kemudian sequalize create dan database wayshub sudah dibuat
<img width="574" alt="Screenshot 2023-04-07 at 15 25 41" src="https://user-images.githubusercontent.com/102456153/230804552-d783a39e-3470-4c6f-965a-678f7ff3d699.png">

- Coba masuk ke MYSQL dan database wayshub telah berhasil dibuat
<img width="574" alt="Screenshot 2023-04-07 at 15 30 01" src="https://user-images.githubusercontent.com/102456153/230804568-cae5d5b3-7e59-4c9d-ba82-ed37ad9ec4cc.png">

- Dikarenakan masih kosong table wayshub, lakukan ``sequelize db:migrate`` dimana fitur-fitur yang ada di wayshub bisa tertransfer ke databese 
<img width="576" alt="Screenshot 2023-04-07 at 15 32 34" src="https://user-images.githubusercontent.com/102456153/230804570-9552cc21-ba6d-4769-9f3e-4d1eb9d9b1d5.png">

- Berikut tampilan MYSQL wayshub setelah di migrate
<img width="578" alt="Screenshot 2023-04-07 at 15 34 39" src="https://user-images.githubusercontent.com/102456153/230804584-d3d40967-ead5-4bfa-84e0-99b7b1735d34.png">

- Selanjutnya coba lakukan **Sign Up**
<img width="1324" alt="Screenshot 2023-04-07 at 15 40 41" src="https://user-images.githubusercontent.com/102456153/230804613-bd38ba15-1a3b-4fce-9fff-473b10bbb0be.png">

- Berikut tampilan setelah saya sudah melakukan **Sign In**
<img width="1323" alt="Screenshot 2023-04-07 at 15 41 42" src="https://user-images.githubusercontent.com/102456153/230804618-1ce30153-8972-448f-89c2-71ad59b9c2db.png">

- Pada database nya, sudah terjadi penambahan pada table Chanels dimana berhasil membuat akun baru
<img width="577" alt="Screenshot 2023-04-07 at 15 46 31" src="https://user-images.githubusercontent.com/102456153/230804624-8607df49-38b7-4572-92ee-e7be720500d8.png">


## 2. Gateway NGINX
- Pertama saya akses server gateway di terminal
<img width="578" alt="Screenshot 2023-04-06 at 16 56 26" src="https://user-images.githubusercontent.com/102456153/230804678-21561c7b-50f9-4485-83fe-72392b5a0c6d.png">

- Install nginx sebagai web server untuk aplikasi saya
<img width="576" alt="Screenshot 2023-04-06 at 16 59 06" src="https://user-images.githubusercontent.com/102456153/230804680-805c62da-0453-4f53-89a4-ec7b37468aba.png">

- Kemudian saya membuat domain frontend dan backend wayshub di cloudflare 
<img width="1402" alt="Screenshot 2023-04-06 at 17 04 27" src="https://user-images.githubusercontent.com/102456153/230804688-3681bd10-9586-492d-bfde-c680d4f1aadd.png">

- Setelah itu buat reverse proxy untuk frontend dan backend wayshub
<img width="578" alt="Screenshot 2023-04-06 at 17 12 53" src="https://user-images.githubusercontent.com/102456153/230804721-7a46f009-a9d2-4cbf-bca0-595600330415.png">
<img width="574" alt="Screenshot 2023-04-06 at 17 17 02" src="https://user-images.githubusercontent.com/102456153/230804728-f053b422-5ae3-4b82-980b-28f01220df5a.png">

- Reload nginx karena sudah melakukan perubahan
<img width="579" alt="Screenshot 2023-04-06 at 17 18 11" src="https://user-images.githubusercontent.com/102456153/230804752-33d4958f-6ad0-48de-b9ff-4548ec674d67.png">

- Buat PM2 ecosystem untuk frontend dan backend.
<img width="577" alt="Screenshot 2023-04-06 at 17 32 00" src="https://user-images.githubusercontent.com/102456153/230804763-5022174e-5ea0-4f23-845f-4a49a5ff2e38.png">
<img width="578" alt="Screenshot 2023-04-06 at 17 33 21" src="https://user-images.githubusercontent.com/102456153/230804765-9115d31e-e84b-4278-86f0-bef8409a2ffe.png">

- Coba jalankan PM2 wayshub frontend dan backend menggunakan domain 
<img width="579" alt="Screenshot 2023-04-06 at 17 44 41" src="https://user-images.githubusercontent.com/102456153/230804773-4884dd13-4b2f-4e3d-97c8-f80129695691.png">

- Wayshub frontend dan backend telah berhasil diakses melalui domain
<img width="1324" alt="Screenshot 2023-04-06 at 17 51 08" src="https://user-images.githubusercontent.com/102456153/230804810-d2fab9c8-e852-4988-a38a-cbce0adcefdd.png">
<img width="1326" alt="Screenshot 2023-04-06 at 17 51 43" src="https://user-images.githubusercontent.com/102456153/230804815-e6189269-ccad-4792-8810-ce9f81fedc56.png">

