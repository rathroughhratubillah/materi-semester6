# Membuat Billing Allert Di aws untuk menghindari kelebihan Alokasi Dana

1. Menu Dashboard AWS Kita Pilih billing preference untuk mengaktifkan allert
masuk billing and cost managemet
pada menu cost manajemen scroll kebawah pilih billing preferences
pilih menu alert preferences klik edit
isi email ceklis receive
klik update

![alt text](image-20.png)

masuk menu cloudwatch
all services pilih cloudwatch
![alt text](image-9.png)


pilih menu create alarm
![alt text](image-11.png)

pastikan region aada di us virginia > KLIK menu create alert > Klik matric > klik menu biling

![alt text](image-12.png)
![alt text](image-13.png)


klik menu total estimatedcharge,pilih / ceklis mata uang usd
![alt text](image-14.png)


beri nama allert= NIM_BillingAlert > conditions static>greathertha>1 usd

![alt text](image-15.png)


create new topic > Nim_BillingAllert> select an existing sns topic
![alt text](image-17.png)


klik next, alarm name> Nim_BillingAllert, Create Alarm
Buka Inbox/ spam email dari asw lalu ketik confirm
![alt text](image-18.png)
![alt text](image-19.png)