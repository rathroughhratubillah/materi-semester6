Start Instance di AWS EC2
Patching OS -> sudo apt update && sudo apt upgrade
Install Docker di EC2 AWS https://docs.docker.com/
Uninstall Docker old version (sudo apt remove $(dpkg --get-selections docker.io docker-compose docker-compose-v2 docker-doc podman-docker containerd runc | cut -f1))
Set up Apt Docker
Install Docker Engine
Cek Docker -> systemctl status docker
https://raw.githubusercontent.com/rathroughhratubillah/materi-semester6/e2d37c999fd5536ac3f4fd87b702f3efad805f01/pertemuan11/image-1.png
