## Buat BASH Script untuk Instalasi Node Version Manager!
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
exec bash
nvm install 14
nvm use 14
node -v
nvm -v
```
- Buat **nano nvm.sh**. Kemudian path dan copy curl instalasi nvm. 
<img width="574" alt="Screenshot 2023-03-24 at 14 15 18" src="https://user-images.githubusercontent.com/102456153/227456143-9337bde7-8fbe-43c3-8e17-42d6bece87c3.png">

- Script meng-clone nvm ke repository. Dikarenakan saya sudah memiliki repository untuk nvm dan source nya, maka akan keluar seperti ini.
<img width="576" alt="Screenshot 2023-03-24 at 14 15 36" src="https://user-images.githubusercontent.com/102456153/227456152-88a8bd6a-3d15-436f-80f1-819123c865a2.png">

- Untuk memastikan sudah terinstall atau tidak. Jika mengeluarkan **nvm** maka artinya telah berhasil terinstall.
<img width="575" alt="Screenshot 2023-03-24 at 14 42 46" src="https://user-images.githubusercontent.com/102456153/227456372-e197ade0-8d34-4295-a897-5270c82fd4d5.png">

- Kemudian install nvm versi yang diinginkan. 
<img width="575" alt="Screenshot 2023-03-24 at 14 22 04" src="https://user-images.githubusercontent.com/102456153/227456382-58d902e7-8007-4b7c-b06f-4fc3084726e6.png">

- Berikut saya memastikan sudah terinstall dengan cara cek version.
<img width="575" alt="Screenshot 2023-03-24 at 14 23 52" src="https://user-images.githubusercontent.com/102456153/227456399-5ff81fdd-226e-4872-bbcc-8abbf88c0592.png">


## Jalankan Aplikasi NodeJS (Dumbflix) dengan Status ufw Enable!
- Masuk ke dalam directory dumbflix dan aktifkan firewall
<img width="574" alt="Screenshot 2023-03-21 at 08 18 44" src="https://user-images.githubusercontent.com/102456153/226498485-b76609eb-1cee-4d29-8b42-994a193ae712.png">

- Jalankan aplikasi Dumbflix
<img width="577" alt="Screenshot 2023-03-21 at 08 19 20" src="https://user-images.githubusercontent.com/102456153/226498488-46bdbdaf-4aeb-42e7-8cfe-c2b896a09748.png">

- Dumbflix sudah dapat diakses di browser
<img width="1322" alt="Screenshot 2023-03-21 at 08 19 35" src="https://user-images.githubusercontent.com/102456153/226498495-b700dc17-880a-47cc-9e04-654f5f571a93.png">
