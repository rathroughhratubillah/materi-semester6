# Membuat Vm /Instance di AWS EC2 Dengan AMI

SEARCH lalu cari EC2 LALU BUKA Menu EC2 keliatan dashboard
![alt text](image-21.png)

klik menu launch instancee > setting region ke singapur> klik launch instance> isi name di name and tags NIM_server6A> k
![alt text](image-22.png)
![alt text](image-23.png)

instance type trs search free tier eligible t3.micro
mrmbuat key fair > create new key pair>beri nama NIM_server6A>RSA>.pem>create key pair
nanti kedownload private key pair
![alt text](image-25.png)
![alt text](image-26.png)
![alt text](image-27.png)
![alt text](image-28.png)


network setting/securoty > create security group>pallow ssh trafic form dan allow semua>pilih anywhereanywhere> storage setting> configure storage > 30gb 9p3

![alt text](image-30.png)
klik launch instance
![alt text](image-31.png)
![alt text](image-32.png)
![alt text](image-33.png)