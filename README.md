https://docs.gitlab.com/ee/install/docker/installation.html


docker compose up -d


Gitlab url: http://localhost:80

username: root
password: cat /etc/gitlab/initial_root_password


# Clone a repo
git clone http://localhost/root/helloworld.git


# Docker compose set limits
https://www.google.com/search?q=docker+compose+increase+memory
https://stackoverflow.com/questions/42345235/how-to-specify-memory-cpu-limit-in-docker-compose-version-3


# -------------------------
# Delete Docker build cache
# -------------------------
docker builder prune



# Open resolv.conf
vim /etc/resolv.conf

# Add Google nameserver
nameserver 8.8.8.8



# Check status (Powershell) of the Docker container
while(1){ docker ps -a;start-sleep -seconds 5;clear }




# ------------------------------
# Create ssh key pair on Windows
# ------------------------------

mkdir C:/Users/TO11RC/.ssh

# Choose id_rsa as filename
ssh-keygen -t rsa -b 2048 -C "Used for my local Gitlab Docker instance"


# Test
ssh -vT git@localhost


# Clone repo using SSH
git clone git@localhost:root/hellogitlab.git


# Add ssh public key to Gitlab
> Edit profile > SSH Keys > Add new key