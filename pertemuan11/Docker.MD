Start Instance di AWS EC2
Patching OS -> sudo apt update && sudo apt upgrade
Install Docker di EC2 AWS https://docs.docker.com/
Uninstall Docker old version (sudo apt remove $(dpkg --get-selections docker.io docker-compose docker-compose-v2 docker-doc podman-docker containerd runc | cut -f1))
Set up Apt Docker
Install Docker Engine
Cek Docker -> systemctl status docker

pertemuan11/image-1.png

