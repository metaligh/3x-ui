3x-ui VLESS REALITY installation + Docker script from video
https://www.youtube.com/watch?v=VyfhVNUH8C8

0) Buy Your hosting, get root login and root password. https://aeza.net/?ref=554977

1) Install https://mobaxterm.mobatek.net/download.html and connect to your Server IP.

2) Update, upgrade server:
sudo apt update && sudo apt -y upgrade

3) Install Docker: 
wget https://raw.githubusercontent.com/docker/docker-install/master/install.sh && chmod +x install.sh && ./install.sh

4) Go to: 
https://hub.docker.com/repository/docker/metaligh/3x-ui/general

5) Make 3xua docker container config:
mkdir /opt/3xui
cd /opt/3xui
touch docker-compose.yml
nano docker-compose.yml

6) Shift + Insert configuration yml from https://hub.docker.com/repository/docker/metaligh/3x-ui/general
Ctrl + X... y... Enter

7) Start container 3x-ui
docker compose up -d

8) ss -tulnp - Check port 2053

9) Make secure tonnel drom your server to your computer on port 2053 in mobaxterm.
Tunneling -> Port 2053 -> your Server IP login root port 22... your server ip port 2053

10) Go to http://localhost:2053 login admin password admin and change your configuration.

11) Make your own settings

12) Download and install https://github.com/hiddify/hiddify-next/releases 
Copy and past your config and that is all. Enjoy!
