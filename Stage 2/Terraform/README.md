## Terraform 


- Buat directory untuk server IDCloudHost
<img width="572" alt="Screenshot 2023-05-03 at 03 33 18" src="https://user-images.githubusercontent.com/102456153/236295572-59ecfabb-bb4c-46c1-8621-fe082ced9d25.png">

- Kemudian membuat script terraform **main.tf** di dalam directory yang telah dibuat
<img width="814" alt="Screenshot 2023-05-07 at 10 04 05" src="https://user-images.githubusercontent.com/102456153/236655512-3f030c39-7d23-4f2b-9b81-f0af257fec20.png">

<img width="572" alt="Screenshot 2023-05-07 at 09 29 11" src="https://user-images.githubusercontent.com/102456153/236655405-4dfb9885-62fe-4b15-8ba6-487416ea2727.png">



- Setelah itu, lakukan `terraform init` untuk initialize script
<img width="732" alt="Screenshot 2023-05-03 at 04 09 31" src="https://user-images.githubusercontent.com/102456153/236295715-065d5c5f-1631-4efb-8d70-8e5347fde623.png">

- Sekarang lakukan `terraform plan` dan jika script berhasil, akan keluar seperti ini 
<img width="751" alt="Screenshot 2023-05-07 at 18 38 09" src="https://user-images.githubusercontent.com/102456153/236675373-48b93354-7090-4cb8-8eaf-b7e4ac9c6691.png">


<img width="733" alt="Screenshot 2023-05-03 at 04 15 05" src="https://user-images.githubusercontent.com/102456153/236296137-63489f87-32b7-41b1-88a6-c529a065bc4a.png">
<img width="732" alt="Screenshot 2023-05-03 at 04 15 08" src="https://user-images.githubusercontent.com/102456153/236296149-4dd5bd0a-68f3-4ef6-80bc-93ee58d41a2a.png">
<img width="733" alt="Screenshot 2023-05-03 at 04 15 17" src="https://user-images.githubusercontent.com/102456153/236296293-6e821ed0-9350-4355-8eec-b7c33be37a1b.png">

- Selanjutnya lakukan `terraform apply` dan ketik *yes* untuk dijalankan
<img width="734" alt="Screenshot 2023-05-03 at 04 16 25" src="https://user-images.githubusercontent.com/102456153/236296384-9cf941ac-ca77-4e70-9fab-8adf86677133.png">
<img width="696" alt="Screenshot 2023-05-07 at 18 42 05" src="https://user-images.githubusercontent.com/102456153/236675368-50e31d9a-b7eb-4e5f-ab9f-7e691fe77cfa.png">


- Server **appserver**, **gateway**, **monitoring** dan **floting IP** telah berhasil dibuat
<img width="1320" alt="Screenshot 2023-05-07 at 18 37 34" src="https://user-images.githubusercontent.com/102456153/236675284-608bceba-0caf-4ec2-b496-b8f503966405.png">
<img width="1320" alt="Screenshot 2023-05-07 at 18 37 38" src="https://user-images.githubusercontent.com/102456153/236675293-90112554-1cea-44f1-a7e9-31de8e4546cb.png">
<img width="1316" alt="Screenshot 2023-05-07 at 18 37 42" src="https://user-images.githubusercontent.com/102456153/236675303-d473e180-56d9-45fe-89dc-2779fcf6cd8b.png">
<img width="394" alt="Screenshot 2023-05-07 at 18 37 47" src="https://user-images.githubusercontent.com/102456153/236675308-4b48405f-2966-4e3d-ac2f-571e227b8f02.png">

 


