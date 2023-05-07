## Terraform 


- Buat directory untuk server IDCloudHost
<img width="572" alt="Screenshot 2023-05-03 at 03 33 18" src="https://user-images.githubusercontent.com/102456153/236295572-59ecfabb-bb4c-46c1-8621-fe082ced9d25.png">

- Kemudian membuat script terraform **main.tf** di dalam directory yang telah dibuat
<img width="814" alt="Screenshot 2023-05-07 at 10 04 05" src="https://user-images.githubusercontent.com/102456153/236655454-f2151bce-9975-424b-a2d0-bbfd52747a29.png">

<img width="572" alt="Screenshot 2023-05-07 at 09 29 11" src="https://user-images.githubusercontent.com/102456153/236655405-4dfb9885-62fe-4b15-8ba6-487416ea2727.png">



- Setelah itu, lakukan `terraform init` untuk initialize script
<img width="732" alt="Screenshot 2023-05-03 at 04 09 31" src="https://user-images.githubusercontent.com/102456153/236295715-065d5c5f-1631-4efb-8d70-8e5347fde623.png">

- Sekarang lakukan `terraform plan` dan jika script berhasil, akan keluar seperti ini 
<img width="707" alt="Screenshot 2023-05-07 at 09 29 45" src="https://user-images.githubusercontent.com/102456153/236655372-3298dc2d-135f-461c-aee8-906cd0f0a8f0.png">


<img width="733" alt="Screenshot 2023-05-03 at 04 15 05" src="https://user-images.githubusercontent.com/102456153/236296137-63489f87-32b7-41b1-88a6-c529a065bc4a.png">
<img width="732" alt="Screenshot 2023-05-03 at 04 15 08" src="https://user-images.githubusercontent.com/102456153/236296149-4dd5bd0a-68f3-4ef6-80bc-93ee58d41a2a.png">
<img width="733" alt="Screenshot 2023-05-03 at 04 15 17" src="https://user-images.githubusercontent.com/102456153/236296293-6e821ed0-9350-4355-8eec-b7c33be37a1b.png">

- Selanjutnya lakukan `terraform apply` dan ketik *yes* untuk dijalankan
<img width="734" alt="Screenshot 2023-05-03 at 04 16 25" src="https://user-images.githubusercontent.com/102456153/236296384-9cf941ac-ca77-4e70-9fab-8adf86677133.png">
<img width="781" alt="Screenshot 2023-05-07 at 03 23 17" src="https://user-images.githubusercontent.com/102456153/236645266-4c317716-9f24-4786-a0c9-3681a0a0091e.png">


- Server **appserver**, **gateway**, **monitoring** dan **floting IP** telah berhasil dibuat
<img width="1316" alt="Screenshot 2023-05-07 at 09 58 50" src="https://user-images.githubusercontent.com/102456153/236655344-eabbd055-b806-4064-96ae-116041f0ad15.png">
<img width="1323" alt="Screenshot 2023-05-07 at 09 58 53" src="https://user-images.githubusercontent.com/102456153/236655346-c26b857a-096f-4b2a-805d-ae0dec11963a.png">
<img width="1323" alt="Screenshot 2023-05-07 at 09 58 55" src="https://user-images.githubusercontent.com/102456153/236655348-3e408a5e-70b0-46da-a139-794bb2189eca.png">
<img width="1325" alt="Screenshot 2023-05-07 at 09 59 01" src="https://user-images.githubusercontent.com/102456153/236655349-431fd4ab-0f6c-48ab-86ed-c2258eaa3eff.png">

