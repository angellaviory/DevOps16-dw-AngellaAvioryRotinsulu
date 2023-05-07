## Terraform 


- Buat directory untuk server IDCloudHost
<img width="572" alt="Screenshot 2023-05-03 at 03 33 18" src="https://user-images.githubusercontent.com/102456153/236295572-59ecfabb-bb4c-46c1-8621-fe082ced9d25.png">

- Kemudian membuat script terraform **main.tf** di dalam directory yang telah dibuat
<img width="814" alt="Screenshot 2023-05-07 at 10 04 05" src="https://user-images.githubusercontent.com/102456153/236655512-3f030c39-7d23-4f2b-9b81-f0af257fec20.png">

<img width="572" alt="Screenshot 2023-05-07 at 09 29 11" src="https://user-images.githubusercontent.com/102456153/236655405-4dfb9885-62fe-4b15-8ba6-487416ea2727.png">



- Setelah itu, lakukan `terraform init` untuk initialize script
<img width="732" alt="Screenshot 2023-05-03 at 04 09 31" src="https://user-images.githubusercontent.com/102456153/236295715-065d5c5f-1631-4efb-8d70-8e5347fde623.png">

- Sekarang lakukan `terraform plan` dan jika script berhasil, akan keluar seperti ini 
<img width="725" alt="Screenshot 2023-05-07 at 10 29 41" src="https://user-images.githubusercontent.com/102456153/236656303-d037b097-9bbc-45c0-8cab-3d6296ddcf27.png">

<img width="733" alt="Screenshot 2023-05-03 at 04 15 05" src="https://user-images.githubusercontent.com/102456153/236296137-63489f87-32b7-41b1-88a6-c529a065bc4a.png">
<img width="732" alt="Screenshot 2023-05-03 at 04 15 08" src="https://user-images.githubusercontent.com/102456153/236296149-4dd5bd0a-68f3-4ef6-80bc-93ee58d41a2a.png">
<img width="733" alt="Screenshot 2023-05-03 at 04 15 17" src="https://user-images.githubusercontent.com/102456153/236296293-6e821ed0-9350-4355-8eec-b7c33be37a1b.png">

- Selanjutnya lakukan `terraform apply` dan ketik *yes* untuk dijalankan
<img width="734" alt="Screenshot 2023-05-03 at 04 16 25" src="https://user-images.githubusercontent.com/102456153/236296384-9cf941ac-ca77-4e70-9fab-8adf86677133.png">
<img width="737" alt="Screenshot 2023-05-07 at 10 29 02" src="https://user-images.githubusercontent.com/102456153/236656264-3a45dd8a-8e09-4c29-bc75-22efd45903ab.png">


- Server **appserver**, **gateway**, **monitoring** dan **floting IP** telah berhasil dibuat
-<img width="1319" alt="Screenshot 2023-05-07 at 10 31 29" src="https://user-images.githubusercontent.com/102456153/236656271-f8183de7-31cc-4eb3-a93f-68d6c1e36443.png">
<img width="1322" alt="Screenshot 2023-05-07 at 10 31 33" src="https://user-images.githubusercontent.com/102456153/236656273-076f4ef4-f24e-4103-bf67-b77c020af8b0.png">
<img width="1322" alt="Screenshot 2023-05-07 at 10 31 36" src="https://user-images.githubusercontent.com/102456153/236656274-3b499c81-06d0-45ec-b36a-21120e4eebef.png">
<img width="385" alt="Screenshot 2023-05-07 at 10 31 40" src="https://user-images.githubusercontent.com/102456153/236656275-0108c11c-1fac-47eb-a11f-a90d1ce8aaf4.png">
 


