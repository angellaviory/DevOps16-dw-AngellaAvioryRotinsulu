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

- Kemudian saya masuk ke dalam file `main.tf` yang didalamnya akan saya isi konfigurasi pembuatan VM dan Floating IP.
<img width="613" alt="Screenshot 2023-05-18 at 02 11 35" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2b4d3ebf-1ec8-45ec-8f9d-ec2538a3547b">
<img width="666" alt="Screenshot 2023-05-17 at 16 00 57" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2cf86522-c302-4884-9cb1-df2baa152475">
<img width="721" alt="Screenshot 2023-05-17 at 06 21 33" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7b06ea1e-fa50-41be-ad40-4e38a9b5d92b">

- Saatnya membuat VM dan Floating IP menggunakan terraform. Langkah pertama adalah melakukan **terraform init**, dimana file `main.tf`akan di initialized.
<img width="680" alt="Screenshot 2023-05-17 at 19 18 11" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/da738ede-99eb-404b-8dd2-99a9be460eb5">


- Jika initialized telah berhasil dilakukan, langkah selanjutnya adalah **terraform plan**, dimana akan menunjukkan rencana pembuatan VM dan Floating IP dari hasil konfigurasi file `main.tf` di IDCloudHost.
<img width="730" alt="Screenshot 2023-05-17 at 09 28 12" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/cd27ee27-7422-4d1d-b385-a7eb54043098">
<img width="660" alt="Screenshot 2023-05-17 at 09 28 29" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/cc9892e2-2e16-4de1-bb4d-66d09aa666d2">
<img width="684" alt="Screenshot 2023-05-17 at 16 20 39" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7bfce9ba-8fb6-4cfe-9fe0-900c5476e3aa">
<img width="684" alt="Screenshot 2023-05-17 at 16 20 46" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/bb59883a-73f1-402b-be1a-d3461b089423">
<img width="685" alt="Screenshot 2023-05-17 at 16 20 51" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/0a75ee65-ff79-44ff-b7c3-65e5e71ae112">
<img width="687" alt="Screenshot 2023-05-17 at 16 20 56" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/8ec9c217-f35a-4418-859d-cca11897f8d5">


- Langkah terakhir adalah melakukan **terraform apply**, dimana setelah memberikan value **yes** maka terraform akan membuat VM dan Floating IP di IDCloudHost.
<img width="692" alt="Screenshot 2023-05-17 at 16 06 19" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/c7022353-abc5-4f03-8a87-d71643a13cac">
<img width="639" alt="Screenshot 2023-05-17 at 19 26 41" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/56766973-94e8-43ba-9eb2-b9aac9f4b902">

- Server telah berhasil dibuat dengan terraform. Berikut saya sudah bisa mengakses server tanpa memasukkan ssh.
<img width="737" alt="Screenshot 2023-05-17 at 19 28 39" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/424c13cb-8199-43f7-b186-79b41b101860">
<img width="773" alt="Screenshot 2023-05-17 at 19 29 23" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/95148f96-bd9d-4797-b555-73e980ec62d9">
<img width="701" alt="Screenshot 2023-05-17 at 19 30 42" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/9f0ec57c-2adb-4783-9e34-9cdfc3370c59">
<img width="745" alt="Screenshot 2023-05-17 at 19 31 37" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/9cecb490-fdb8-458a-974d-7f6a208b696b">


# Ansible

- Sebelum melakukan instalasi ansible, saya akan mendownload package manager **pip** untuk digunakan sebagai python interpreter dan python environment user.
<img width="622" alt="Screenshot 2023-05-17 at 06 28 37" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7c6bdc62-9ac2-4ba9-ab3e-4e796a93d957">
<img width="690" alt="Screenshot 2023-05-17 at 07 28 24" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/65da208a-f03f-4b28-9141-636b0089cb83">
<img width="725" alt="Screenshot 2023-05-17 at 07 31 38" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/5867711f-9daf-42d0-b41a-a2b2bddd6347">

- Kemudian Install ansible.
<img width="725" alt="Screenshot 2023-05-17 at 07 32 25" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/b218b728-804c-44c1-8920-d110d0d8926b">

- Untuk memastikan ansible telah terinstall dengan menggunakan command `ansible --version`.
<img width="728" alt="Screenshot 2023-05-17 at 08 38 45" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a705fbb7-e74d-4662-a5fe-2f4600dbc4c5">

- Sekarang saya akan memasukkan private-key `id_rsa` lokal saya ke VM multipass saya.
<img width="783" alt="Screenshot 2023-05-18 at 02 49 28" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/4093fc97-c7a2-4f4c-b953-b465414d3869">

- Setelah ansible sudah terinstall, saya sudah bisa membuat berbagai macam konfigurasi. Pertama-tama yang akan saya lakukan adalah membuat directory.
<img width="666" alt="Screenshot 2023-05-18 at 02 20 23" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/183e2576-f054-416e-ad33-fcdf04ee6fa8">

- Kemudian saya akan membuat file `Inventory` yang berisikan **server** dengan alamat IP nya dan **variabel** berisikan username saya dan lokasi python interpreter saya disimpan.
<img width="666" alt="Screenshot 2023-05-18 at 02 22 23" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/ca6752a8-c15d-49f4-8e8f-dd20c5ed4eae">

- Kemudian saya akan membuat file `ansible.cfg`, yang berisikan *default*. Disini invenetory akan diarahkan ke file **Inventory**, memberitahukan lokasi private-key saya berada, Meng-skip finger print dan python interpreter menjadi auto silent.
<img width="664" alt="Screenshot 2023-05-18 at 02 23 35" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/db992c59-fe83-4e96-b360-1dfd04ac3334">

## Appserver
- Berikut konfigurasi setup docker untuk server appserver dalam bentuk yaml file.
<img width="760" alt="Screenshot 2023-05-18 at 02 45 45" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/bc4528e9-7a66-47de-8cfc-e3cbc741c3e5">

## Gateway
- Berikut konfigurasi setup docker untuk server gateway dalam bentuk yaml file.
<img width="755" alt="Screenshot 2023-05-18 at 02 46 05" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/09486b2e-5dfd-4592-85d0-b4256d85445f">

## CI/CD
- Berikut konfigurasi setup docker untuk server cicd dalam bentuk yaml file.
<img width="761" alt="Screenshot 2023-05-18 at 02 46 11" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/1e4e322f-aba1-49f0-bc94-3b7fd5ac35e5">

## Monitoring
- Berikut konfigurasi setup docker untuk server monitoring dalam bentuk yaml file.
<img width="759" alt="Screenshot 2023-05-18 at 02 46 18" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2d4a1a18-59d9-444c-91af-f8a5a9752eb4">


