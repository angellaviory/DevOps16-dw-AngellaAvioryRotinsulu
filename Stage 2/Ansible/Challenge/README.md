## Login melalui SSH-Key
- Masukkan `key-public` local ke appserver (authorized_key)
<img width="570" alt="Screenshot 2023-05-07 at 20 28 34" src="https://user-images.githubusercontent.com/102456153/236693238-fb6a6b3f-6e74-4909-8cbd-15730e23122c.png">

- Kemudian masukkan `private-key` local ke file `private-key` server ansible
<img width="571" alt="Screenshot 2023-05-07 at 20 32 11" src="https://user-images.githubusercontent.com/102456153/236693239-89b45fda-7b70-464b-b700-5792622b5685.png">

- Sekarang dapat mengakses appserver tanpa menggunakan password
<img width="591" alt="Screenshot 2023-05-07 at 20 30 07" src="https://user-images.githubusercontent.com/102456153/236693244-eed36cb7-d190-4d0e-911c-3b64d6d56019.png">

## App Deployment dengan Docker-Compose

## Domain SSL using OpenSSL dengan Ansible
