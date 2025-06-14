# DOCKER_COMPOSE_EXECUTANDO

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04


sudo apt update

sudo apt install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] 

https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update

apt-cache policy docker-ce

sudo apt install docker-ce

sudo systemctl start docker

sudo systemctl status docker

sudo apt  install docker-compose 

mkdir -p ~/.docker/cli-plugins/

curl -SL https://github.com/docker/compose/releases/download/v2.27.1/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose

hmod +x ~/.docker/cli-plugins/docker-compose

docker compose version

sudo apt install maven

java -version

sudo apt-get install openjdk-17-jdk 

sudo update-alternatives --config java

## OUTROS

remover todos os containers: docker system prune -a

sudo lsof -i tcp:8080

kill -9 PID 

sudo docker rm $(sudo docker ps -a -q)

## OPCIONAL

sudo usermod -aG docker ${USER}

su - ${USER}

groups

sudo usermod -aG docker username



