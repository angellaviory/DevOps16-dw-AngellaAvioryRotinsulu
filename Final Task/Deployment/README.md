# fe-dumbmerch
- Hal pertama saya lakukan adalah mengclone aplikasi dari repository github.
<img width="579" alt="Screenshot 2023-05-19 at 03 14 32" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/83450932-d901-4253-ac22-ee1969c7ab1e">

- Kemudian langkah berikutnya adalah menginstall **NVM (Node Version Manager)** yang merupakan engine Node.js. Berikut langkah-langkah yang perlu dilakukan.
```
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
$ exec bash
$ nvm install 16
$ nvm use 16
```
<img width="689" alt="Screenshot 2023-05-19 at 03 49 20" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/11452e0a-ad77-4a40-a2b3-3935caf1d467">
<img width="695" alt="Screenshot 2023-05-19 at 03 50 21" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/5ae33189-aa0e-46cf-af71-33402b42f743">

- Untuk memastikan NVM dan NPM sudah terinstall, bisa melakukan command `node -v`  dan `npm -v` untuk mengetahui versi ke berapa nvm dan npm nya.
<img width="655" alt="Screenshot 2023-05-19 at 03 51 18" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/1b300390-87c7-408e-9cce-746c7e362e19">

- Kemudian saya menginstall framework Node.js yaitu **Express.js**.
<img width="685" alt="Screenshot 2023-05-19 at 03 54 54" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/d6b8eed4-c400-4e5e-b992-06ee44e39151">

- Selanjutnya saya akan membuat file **.env** (environment), dimana saya akan memasukkan IP sehingga aplikasi dapat diakses.


- Sekarang saya sudah bisa mengakses aplikasi fe-dumbmerch. Saya jalankan command `npm start` dan aplikasi berhasil saya mengakses dari browser dengan menggunakan IP:3000.
<img width="1321" alt="Screenshot 2023-05-19 at 03 55 57" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/c5548bd1-0eb1-402c-a5b6-794313dc4600">



# be-dumbmerch
- Hal pertama saya lakukan adalah mengclone aplikasi dari repository github.
<img width="579" alt="Screenshot 2023-05-19 at 03 14 32" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/c8b5dffd-905b-4de9-b844-6eb6bb21cbfd">

- Karena aplikasi menggunakan *Golang*, maka saya akan menginstall Golang terlebih dahulu. Berikut command yang saya gunakan untuk menginstall Golang.
```
(Dalam Directory be-dumbmerch)
$ wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su
$ rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit
$ exec bash

(Diluar Directory be-dumbmerch)
$ sudo nano .bashrc
$ export PATH=$PATH:/usr/local/go/bin
```
<img width="679" alt="Screenshot 2023-05-19 at 05 51 26" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/e894fc71-d501-4f33-96d0-6e60d41dce6a">
<img width="583" alt="Screenshot 2023-05-19 at 06 23 14" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a11ce9ef-7a5f-4d15-95ee-314c3079b57e">
<img width="571" alt="Screenshot 2023-05-19 at 06 18 20" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/622aa354-e5a3-4282-bd81-d821e133d2ca">

- Golang sudah berhasil di install. Saya akan memastikannya dengan meakukan command `go version`.
<img width="579" alt="Screenshot 2023-05-19 at 06 23 48" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/d109f077-72e8-4783-b43a-616d1daab872">



