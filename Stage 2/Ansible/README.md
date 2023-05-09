## SSH
### 1. ubuntu
* Memuat file `id_rsa` di directory ssh dan masukkan `id_rsa` local ke dalam file tersebut
<img width="626" alt="Screenshot 2023-05-10 at 00 09 49" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/6d0a7c78-fa7e-49de-a8ab-5e3aaf619db0">

### 2. appserver
* Masukkan `id_rsa.pub` local ke file `authorized_keys` yang ada di **appserver**
<img width="587" alt="Screenshot 2023-05-09 at 23 59 35" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/6341f20e-acc5-462f-895e-36aef58f057f">

### 3. gateway
* Masukkan `id_rsa.pub` local ke file `authorized_keys` yang ada di **gateway**
<img width="590" alt="Screenshot 2023-05-10 at 00 00 39" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a6ea71b8-c46f-4ae3-87be-a5b4db987be0">

## Inventory
<img width="629" alt="Screenshot 2023-05-10 at 00 19 09" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/4b6ea94b-fec0-41fb-9bb4-2b429f09dd73">

## `ansible.cfg`
<img width="627" alt="Screenshot 2023-05-10 at 00 19 19" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/696bf20d-e4ae-4137-bf49-f41929496eda">



# Appserver
### Instalasi Docker dan Menjalankan Applikasi Wayshub-frontend
- Buat file YAML `docker.yml`
<img width="775" alt="Screenshot 2023-05-10 at 00 50 49" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/e2b1194c-2176-411a-8373-c6bba1e74ae5">

- Jalankan playbook docker
<img width="731" alt="Screenshot 2023-05-10 at 00 50 22" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7dcedd26-6834-43bf-9720-55dd011e577f">

- Setup docker menggunakan ansible sudah berhasil dilakukan
<img width="594" alt="Screenshot 2023-05-10 at 00 55 22" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a36d9d96-2195-45fc-a7b9-39a3f8e744ac">

- Coba pull wayshub-frontend dan run aplikasi tersebut
<img width="610" alt="Screenshot 2023-05-10 at 00 58 35" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/d4a825e0-0f4a-4254-96b9-0bfba5e8121a">

- Wayshub-frontend telah berhasil di akses di browser
<img width="1325" alt="Screenshot 2023-05-10 at 00 59 14" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/9b48f8df-504a-4c2e-a40e-f29a4f4013dc">

### Membuat User Baru dan Menjalankan Konfigurasi Ansible
- Pertama buat file YAML untuk penambahan user baru dan perubahan file `docker.yml`
<img width="632" alt="Screenshot 2023-05-10 at 01 45 48" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a775cd2c-fae9-48c6-8843-36cdc83ede9d">
<img width="786" alt="Screenshot 2023-05-10 at 01 46 46" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/b6b103c3-4e6a-4341-b10e-c2ace33c6a26">

- Jalankan ansible playbook 
<img width="671" alt="Screenshot 2023-05-10 at 01 49 11" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/6345fb5b-ebc1-4f06-8537-2867bd0b780d">


- User telah berhasil ditambahkan
<img width="656" alt="Screenshot 2023-05-10 at 01 04 56" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/716b106f-5f62-4770-b644-4ff42a9e4bd6">

- Mencoba menjalankan wayshub-frontend menggunakan user baru
<img width="736" alt="Screenshot 2023-05-10 at 01 11 47" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/09866a32-1c98-4e91-8636-242bbe108e95">

<img width="1325" alt="Screenshot 2023-05-10 at 00 59 14" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/a3cc8921-27cb-4bef-a5fc-14daff8c62d4">


# Gateway
<img width="590" alt="Screenshot 2023-05-10 at 00 00 39" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/d2ae269e-400a-433f-b99d-599c24d09cba">

### Instalasi NGINX dan Konfigurasi NGINX dan Reverse Proxy beserta Domain
- Pertama buat file YAML `nginx.yml` untuk instalasi nginx 
<img width="672" alt="Screenshot 2023-05-10 at 01 49 36" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/4a2fbe32-22e9-4d75-bd72-7f792b87d9e3">


- Buat directory untuk reverse proxy. Kemudian membuat file `rproxyy.conf` yang berisikan domain
<img width="634" alt="Screenshot 2023-05-10 at 01 32 04" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/085102d8-8e2f-4b49-8e81-51bf6ace33c0">

- Jalankan ansible playbook
<img width="637" alt="Screenshot 2023-05-10 at 01 26 23" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2740287d-c45f-4718-bdf6-a23cde6aa5f5">

- Memastikan nginx telah terinstall dan dapat diakses menggunakan domain
<img width="1322" alt="Screenshot 2023-05-10 at 01 29 37" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/4e522b82-591b-4c32-a24a-d683006372d3">

### Membuat User Baru dan Menjalankan Konfigurasi Ansible
- Pertama buat file YAML untuk penambahan user baru dan perubahan file `nginx.yml`
<img width="631" alt="Screenshot 2023-05-10 at 01 45 55" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/08123be4-fd0c-4244-a93a-70bef3140c94">
<img width="674" alt="Screenshot 2023-05-10 at 01 49 38" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7eff92d6-a4ae-4119-bdb6-fc825d365c01">


- Jalankan ansible playbook 
<img width="752" alt="Screenshot 2023-05-10 at 01 50 55" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/67603b9e-e569-449a-9ad7-d0131145f53b">

- User telah berhasil ditambahkan
<img width="585" alt="Screenshot 2023-05-10 at 01 39 06" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/4fe13d92-9246-4e12-b2ef-6fb4faa180a5">

- Mencoba menjalankan wayshub-frontend menggunakan user baru
<img width="1322" alt="Screenshot 2023-05-10 at 01 29 37" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/8bc73d76-7c39-4f1f-84cc-a770c2e8be51">
