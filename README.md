# DOCKER_COMPOSE_EXECUTANDO

mkdir -p ~/.docker/cli-plugins/
curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose

chmod +x ~/.docker/cli-plugins/docker-compose

docker compose version

----
sudo rm /usr/local/bin/docker-compose

sudo pip uninstall docker-compose

sudo apt install docker-compose

sudo apt-get -y install python-pip

sudo pip install docker-compose

