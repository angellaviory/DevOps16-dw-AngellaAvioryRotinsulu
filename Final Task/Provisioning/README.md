# Terraform
- Pertama, lakukan instalasi terraform. Saya akan menjalankan command ini untuk menginstall terraform untuk OS Linux di local saya.
<img width="617" alt="Screenshot 2023-05-17 at 06 23 04" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/09825eb2-4336-4c19-860b-910361be65c5">
<img width="901" alt="Screenshot 2023-05-17 at 06 26 12" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/93d3235d-4118-425c-99ed-d994703cbce4">

- Setelah berhasil di install, untuk memastikan saya akan lakukan pengecekkan dengan command `terraform version`.
<img width="628" alt="Screenshot 2023-05-17 at 06 27 55" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2caa0755-c0bf-43fc-9b45-d3682f222352">

- Sebelum saya membuat konfigurasi, saya akan membuat token di IDCloudHost.
<img width="1321" alt="Screenshot 2023-05-17 at 05 54 22" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/b791eefe-f760-47c4-a04f-21158651ea4c">

- Sekarang saya akan membuat VM menggunakan provider IDCloudHost. Pertama-tama, saya akan membuat directory **idch** dan file bernama **main.tf**.
<img width="582" alt="Screenshot 2023-05-17 at 05 51 25" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/b90e2acc-2219-47bc-b082-95c9b336506a">

- Kemudian saya masuk kedalam file `main.tf` yang didalamnya akan saya isi konfigurasi pembuatan VM dan Floating IP.
<img width="776" alt="Screenshot 2023-05-17 at 06 20 10" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/acbb3bbc-17ae-4b8b-b00b-dd5ee5e152c0">
<img width="650" alt="Screenshot 2023-05-17 at 07 15 45" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/34693872-ea8f-44a6-b183-e74aeecc044d">
<img width="721" alt="Screenshot 2023-05-17 at 06 21 33" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7b06ea1e-fa50-41be-ad40-4e38a9b5d92b">


# Ansible
- Sebelum melakukan instalasi ansible, saya akan mendownload package manager **pip** untuk digunakan sebagai python interpreter dan python environment user.
<img width="622" alt="Screenshot 2023-05-17 at 06 28 37" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7c6bdc62-9ac2-4ba9-ab3e-4e796a93d957">
<img width="690" alt="Screenshot 2023-05-17 at 07 28 24" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/65da208a-f03f-4b28-9141-636b0089cb83">
<img width="725" alt="Screenshot 2023-05-17 at 07 31 38" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/5867711f-9daf-42d0-b41a-a2b2bddd6347">

- Kemudian Install ansible.
<img width="725" alt="Screenshot 2023-05-17 at 07 32 25" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/b218b728-804c-44c1-8920-d110d0d8926b">

- Untuk memastikan ansible telah terinstall dengan menggunakan command `ansible --version`.
<img width="728" alt="Screenshot 2023-05-17 at 08 38 45" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a705fbb7-e74d-4662-a5fe-2f4600dbc4c5">

- 
