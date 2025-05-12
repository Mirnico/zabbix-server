# Update 
sudo apt update && sudo apt install -y curl ca-certificates gnupg lsb-release

# Agregar repositorio de Docker
curl -fsSL https://download.docker.com/linux/$(. /etc/os-release; echo "$ID")/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker.gpg
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker.gpg] https://download.docker.com/linux/$(. /etc/os-release; echo "$ID") \
  $(lsb_release -cs) stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Instalar Docker y Docker Compose plugin
sudo apt update && sudo apt install -y docker-ce docker-ce-cli containerd.io docker-compose-plugin

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




