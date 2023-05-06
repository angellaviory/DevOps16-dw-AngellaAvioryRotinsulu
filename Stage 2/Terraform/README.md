## Terraform 


- Buat directory untuk server IDCloudHost
<img width="572" alt="Screenshot 2023-05-03 at 03 33 18" src="https://user-images.githubusercontent.com/102456153/236295572-59ecfabb-bb4c-46c1-8621-fe082ced9d25.png">

- Kemudian membuat script terraform **main.tf** di dalam directory yang telah dibuat
<img width="734" alt="Screenshot 2023-05-03 at 04 04 53" src="https://user-images.githubusercontent.com/102456153/236295583-d25a7488-251d-48f1-a467-16fa9e7cdd68.png">
<img width="735" alt="Screenshot 2023-05-03 at 04 04 59" src="https://user-images.githubusercontent.com/102456153/236295602-d6d68a16-8555-4102-8d22-1258d2c18ddf.png">
<img width="572" alt="Screenshot 2023-05-07 at 03 14 44" src="https://user-images.githubusercontent.com/102456153/236645019-744226f1-5a1b-43de-b2df-3455b48f9dcd.png">


- Setelah itu, lakukan `terraform init` untuk initialize script
<img width="732" alt="Screenshot 2023-05-03 at 04 09 31" src="https://user-images.githubusercontent.com/102456153/236295715-065d5c5f-1631-4efb-8d70-8e5347fde623.png">

- Sekarang lakukan `terraform plan` dan jika script berhasil, akan keluar seperti ini 
<img width="570" alt="Screenshot 2023-05-07 at 03 15 35" src="https://user-images.githubusercontent.com/102456153/236645036-27489a71-29a4-4d37-a386-2a8496599c61.png">
<img width="628" alt="Screenshot 2023-05-07 at 03 15 57" src="https://user-images.githubusercontent.com/102456153/236645040-91c1afd3-a4a9-4d88-b6c7-81e8c749d4fe.png">


<img width="733" alt="Screenshot 2023-05-03 at 04 15 05" src="https://user-images.githubusercontent.com/102456153/236296137-63489f87-32b7-41b1-88a6-c529a065bc4a.png">
<img width="732" alt="Screenshot 2023-05-03 at 04 15 08" src="https://user-images.githubusercontent.com/102456153/236296149-4dd5bd0a-68f3-4ef6-80bc-93ee58d41a2a.png">
<img width="733" alt="Screenshot 2023-05-03 at 04 15 17" src="https://user-images.githubusercontent.com/102456153/236296293-6e821ed0-9350-4355-8eec-b7c33be37a1b.png">

- Selanjutnya lakukan `terraform apply` dan ketik *yes* untuk dijalankan
<img width="734" alt="Screenshot 2023-05-03 at 04 16 25" src="https://user-images.githubusercontent.com/102456153/236296384-9cf941ac-ca77-4e70-9fab-8adf86677133.png">
<img width="781" alt="Screenshot 2023-05-07 at 03 23 17" src="https://user-images.githubusercontent.com/102456153/236645266-4c317716-9f24-4786-a0c9-3681a0a0091e.png">


- Server **appserver**, **gateway**, **monitoring** dan **floting IP** telah berhasil dibuat

<img width="1320" alt="Screenshot 2023-05-07 at 03 20 45" src="https://user-images.githubusercontent.com/102456153/236645185-04f474c8-1f3d-425f-b402-bfc6c4ee8be4.png">
<img width="1317" alt="Screenshot 2023-05-07 at 03 20 49" src="https://user-images.githubusercontent.com/102456153/236645186-5a2308dd-ea7f-4cf2-a159-93f0fb5ac40f.png">
<img width="1316" alt="Screenshot 2023-05-07 at 03 20 52" src="https://user-images.githubusercontent.com/102456153/236645189-0083bd7f-bf02-44b1-871f-92523b279871.png">
<img width="392" alt="Screenshot 2023-05-07 at 03 21 14" src="https://user-images.githubusercontent.com/102456153/236645192-f7363683-5c7f-488a-9be5-e6d5abe1d388.png">



