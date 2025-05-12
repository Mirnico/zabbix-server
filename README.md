Instalar Docker

sudo apt update
sudo apt install -y ca-certificates curl gnupg lsb-release

# Agregar la clave GPG de Docker
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | \
  sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

# Agregar el repositorio oficial
echo \
  "deb [arch=$(dpkg --print-architecture) \
  signed-by=/etc/apt/keyrings/docker.gpg] \
  https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Instalar Docker Engine y Docker Compose
sudo apt update
sudo apt install -y docker-ce docker-ce-cli containerd.io docker-compose-plugin

# Verificar instalación
docker --version
docker compose version


# Clonar repo 

 "" mkdir -p ~/proyectos/zabbix-docker
    cd ~/proyectos/zabbix-docker   ""


 git clone https://github.com/Mirnico/zabbix-server
 cd zabbix-server





# Comandos docker 

# en PC lentas 

COMPOSE_HTTP_TIMEOUT=300 docker-compose up -d


Sino docker-compose up -d


# Zabbix-Server

Ver en "localhost:8080"

USER=Admin

PASSWORD=zabbix




