﻿Aktifkan instance EC2
  
Remote instance menggunakan ssh Powershell dengan format: ssh -i < path-to-key.pem > @IP

Update dan upgrade sistem (sudo apt update && sudo apt upgrade -y)

Install MariaDb (sudo apt install mariadb-server -y)

Cek status MariaDb (sudo systemctl status mariadb)

<img width="1442" height="487" alt="image" src="https://github.com/user-attachments/assets/63d4dfe1-b6ed-4a6b-8f24-785781c0ffd4" />


Test Default Setting database server login sudo mysql -u root -p

<img width="957" height="831" alt="image-1" src="https://github.com/user-attachments/assets/ee364c68-1b96-4652-8cdc-dc91f61924bb" />


Hardening Database Server sudo mysql_secure_installation
Change the password for the root user = Y
Remove anonymous users = Y
Disallow root login remotely = Y
Remove test database and access to it = Y
Reload privilege tables = Y

<img width="833" height="1030" alt="image-6" src="https://github.com/user-attachments/assets/ba5cceca-fedf-4823-abfe-0f7be3ad3ad8" />


Reload privilege tables = Y alt text
Create DB untuk Website Company Profile
Login sebagai root

Create DB nama dbcompro_NIM => CREATE DATABASE dbcompro_NIM;

<img width="444" height="246" alt="image-2" src="https://github.com/user-attachments/assets/43db9273-d335-45d3-80c5-14cb7a9ea662" />

Create User dengan nama = usrcompro_NIM dan password = [PASSWORD] => CREATE USER 'usrcompro_NIM'@'localhost' IDENTIFIED BY '[PASSWORD]'; alt text
Grant user akses ke DB yang baru dibuat => GRANT ALL PRIVILEGES ON dbcompro_NIM.* TO 'usrcompro_NIM'@'localhost';
Flush privileges => FLUSH PRIVILEGES;

<img width="689" height="400" alt="image-4" src="https://github.com/user-attachments/assets/11e37f26-dbd9-4404-9a14-a6b3ad221068" />

exit;
login sebagai usrcompro_NIM dan cek apakah bisa akses ke DB yang baru dibuat

foto
