# DOCKER_COMPOSE_EXECUTANDO

sudo apt update

sudo apt install docker-ce docker-compose-plugin -y

docker --version

sudo usermod -aG docker $USER

              
newgrp docker

                  
docker-compose --version

DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}

mkdir -p $DOCKER_CONFIG/cli-plugins
curl -SL https://github.com/docker/compose/releases/download/v2.36.2/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-plugins/docker-compose

chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose

docker-compose --version
