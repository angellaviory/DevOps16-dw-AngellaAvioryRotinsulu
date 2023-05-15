# SETUP :
## 1. Node-Exporter
<img width="576" alt="Screenshot 2023-05-11 at 18 52 17" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/4b4b4406-742a-46f1-b065-b234849a2553">
<img width="570" alt="Screenshot 2023-05-11 at 19 39 35" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/f28f5a63-c809-401c-becb-d54a1035d18b">
<img width="874" alt="Screenshot 2023-05-11 at 17 27 06" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/7306327a-344a-47b7-8eca-2ec4454b5d63">

## 2. Prometheus
<img width="669" alt="Screenshot 2023-05-15 at 08 10 38" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/384c9fcf-b326-4c16-9733-58639e026fdc">
<img width="804" alt="Screenshot 2023-05-15 at 08 48 59" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/fcc2ce7b-5c5e-42c5-9bfe-a33c2ff898f7">

## 3. Grafana Dashboard
<img width="586" alt="Screenshot 2023-05-15 at 08 36 49" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/99acb14c-3fd0-465f-9d16-45775044685b">
<img width="1310" alt="Screenshot 2023-05-11 at 20 59 36" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/ed9b2c18-72df-4594-968d-016ab28b94ce">


# Install Node-Exporter di Appserver dan Gateway
1. Appserver

<img width="1324" alt="Screenshot 2023-05-11 at 18 51 51" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/5caea609-1dd5-4e0a-9dda-13ff7998868f">

2. Gateway

<img width="1320" alt="Screenshot 2023-05-11 at 19 40 07" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/9ad191a6-d47d-4937-9b68-712bc5b20cd3">

# Grafana:
## Dashboard untuk Monitoring Resourse Server (CPU, RAM, Disk Usage)
Berikut dashboard **appserver**, **gateway**, **monitoring** dan **wayshub-frontend**
<img width="1326" alt="Screenshot 2023-05-12 at 06 44 43" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/54b3d10c-aa7e-458b-a78f-51c0ef957b8c">
<img width="1326" alt="Screenshot 2023-05-12 at 06 44 48" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/e881f69c-79cd-40bc-8109-2f965d03c4c3">
<img width="1318" alt="Screenshot 2023-05-12 at 06 44 54" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/fbf3c1ce-092c-412f-a016-7b3e393e443a">
<img width="1321" alt="Screenshot 2023-05-12 at 06 44 59" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/b9b0ead6-de58-40e3-85f7-f840641b2b9a">

## Alerting Contact Point (Discord, Telegram, dll)
- Membuat contact points ke discord sehingga alerting akan mengirim notification melalui discord
<img width="1311" alt="Screenshot 2023-05-12 at 07 26 34" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/e34238c3-df42-4f71-867b-1e945defd0ce">

- Membuat notification policy
<img width="1316" alt="Screenshot 2023-05-12 at 07 26 27" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/8d347e97-59c1-45bf-a53b-c66e8ba6e0e0">

- Alerting sudah berhasil terhubung dengan discord.
<img width="1313" alt="Screenshot 2023-05-12 at 07 26 07" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/2c8c31a9-d040-4ccd-8f81-ee120a7e6575">


## Alerts: 
1. CPU Usage Over 20%.

<img width="1315" alt="Screenshot 2023-05-15 at 08 32 00" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/ca9cab7d-f488-4556-be40-3b014824a61f">


2. RAM Usage Over 50%
<img width="1317" alt="Screenshot 2023-05-15 at 08 33 26" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/956f3723-4636-49b3-86c1-c72c60c0938b">


3. CPU Usage Over 5%
<img width="1320" alt="Screenshot 2023-05-15 at 08 30 43" src="https://github.com/angellaviory/DevOps16-dw-AngellaAvioryRotinsulu/assets/102456153/50858299-87a5-4f58-84aa-e202c84d6d1d">
