# SSL with Certbot

1. Pertama login ke dalam server gateway nginx melalui terminal. Kemudian lakukan instalasi ``install snapd`` di terminal server gateway.
<img width="574" alt="Screenshot 2023-04-07 at 16 20 44" src="https://user-images.githubusercontent.com/102456153/230643678-1ecaf237-3cb3-4997-be36-c328fea0c697.png">

2. **snapd** telah berhasil di instalasi. Setelah itu, lakukan instalasi core dan refresh core tersebut.
<img width="575" alt="Screenshot 2023-04-07 at 16 21 55" src="https://user-images.githubusercontent.com/102456153/230643687-1160c11c-17e8-4483-9532-14688c476a55.png">

3. Dikarenakan saya menginstalasi menggunakan ``apt``, dimana penginstalan mennggunakan OS package manager. Penghapusan ini dilakukan agar perintah tidak lagi menggunakan ``sudo apt``dapat menggunakan ``sudo snap``.
<img width="573" alt="Screenshot 2023-04-07 at 16 23 12" src="https://user-images.githubusercontent.com/102456153/230643691-d7a642ae-698b-47d4-a1f4-cbbc8cb00479.png">

4. Kemudian install lagi certbot.
<img width="576" alt="Screenshot 2023-04-07 at 16 24 08" src="https://user-images.githubusercontent.com/102456153/230643699-af7644ec-eb26-4b82-94b0-abfbc399f07e.png">

5. Jalankan perintah ``sudo ln -s /snap/bin/certbot /usr/bin/certbot`` agar certbot dapat dijalankan.
<img width="577" alt="Screenshot 2023-04-07 at 16 24 33" src="https://user-images.githubusercontent.com/102456153/230643708-aa8b4284-78a4-4e7f-802e-34ee32c84a74.png">

6. Setelah itu buat setifikat certbot pada nginx, agar website kita aman atau secure.
<img width="576" alt="Screenshot 2023-04-07 at 16 29 34" src="https://user-images.githubusercontent.com/102456153/230643716-44cd8488-1f0e-49f0-9f47-cda865ea8895.png">
<img width="578" alt="Screenshot 2023-04-07 at 16 36 31" src="https://user-images.githubusercontent.com/102456153/230643730-3419ed2b-e2a3-42e2-a453-e17977580751.png">

7. Website sudah berhasil secure. Berikut website baik frontend maupun backend telah berhasil di SSL.
<img width="1325" alt="Screenshot 2023-04-07 at 16 32 21" src="https://user-images.githubusercontent.com/102456153/230643781-8b82e2cd-14b0-40c0-a76b-7a33d1acfcff.png">
<img width="1323" alt="Screenshot 2023-04-07 at 16 35 22" src="https://user-images.githubusercontent.com/102456153/230643784-f24cb122-d2ba-4334-80d0-44d37bdb90e8.png">
<img width="1325" alt="Screenshot 2023-04-07 at 16 32 14" src="https://user-images.githubusercontent.com/102456153/230643788-6eff0bc6-b018-4ce1-b797-d1997f34f9c4.png">
<img width="1324" alt="Screenshot 2023-04-07 at 16 34 47" src="https://user-images.githubusercontent.com/102456153/230643805-eb244082-341d-4305-aaa8-4ea842db2aa2.png">
<img width="1326" alt="Screenshot 2023-04-07 at 16 35 10" src="https://user-images.githubusercontent.com/102456153/230643818-b48f4435-693e-4a07-a8de-f5c7e8899b48.png">
