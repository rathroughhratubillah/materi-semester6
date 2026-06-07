# UAS Administrasi Server : Deploy 2 System Apps Static Web dan Dynamic Web
### 1. Membuat Insteance baru pada AWS Region ap-southeast-1 Singapore
![alt text](image.png)
### 2.  Membuat Project UAS Static & Dynamic
![alt text](image-1.png)
### 3. Install Docker dari repository resmi Docker (jalankan dipowershell)
    "sudo apt update"
    "sudo apt install -y ca-certificates curl gnupg"
    "sudo install -m 0755 -d /etc/apt/keyrings"
    "curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg"
    "sudo chmod a+r /etc/apt/keyrings/docker.gpg"
    ". /etc/os-release"
    "echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download docker.com/linux/ubuntu ${VERSION_CODENAME} stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/ null"
    "sudo apt update"
    "sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin"

    LALU AKTIFKAN DOCKER
    "sudo systemctl enable docker"
    "sudo systemctl start docker"
    "sudo usermod -aG docker ubuntu"

    LALU CEK APAKAH DOCKER BERHASIL DIINSTALL
    "docker --version"
    "docker compose version"
![alt text](image-2.png)
### 4. Set Up Docker Hub
    BUAT REPOSITORY BARU PADA DOCKER HUB
![alt text](image-3.png)

    BUAT PERSONAL ACCES TOKEN
![alt text](image-4.png)
### 5. Login Docker ke EC2 Melalui PowerShell
    "docker login -u gamine1"
    (Saat diminta password, paste Docker Hub access token, bukan password akun biasa.)

    BUILD IMAGE DARI PROJECT
    Pastikan Posisi Folder di (cd ~/uas-cloud)
    lalu build "docker compose build static-cv dynamic-app"
    lalu push image ke docker hub "docker compose push static-cv dynamic-app"
![alt text](image-5.png)
### 6. Set Up Github
    Buat Repository Baru di Github - lalu push
![alt text](image-6.png)
### 7. Set Up Secret Github
![alt text](image-7.png)
### 8. Set up Github Action
![alt text](image-8.png)
### 9. Test Statis
![alt text](image-9.png)
### 10. Test Dynamic
![alt text](image-10.png)