## DOCKER Commands
```bash
########## Executar Containers ##########

# Executar um container
docker run <image_name>

# Executar um container em modo interativo
docker run -it <image_name> /bin/bash

# Executar um container em background (detached mode)
docker run -d <image_name>

########## Visualizar Containers ##########

# Listar containers em execução
docker ps

# Listar todos os containers (inclusive parados)
docker ps -a

# Ver logs de um container
docker logs <container_id>

# Inspecionar detalhes de um container
docker inspect <container_id>

## Build de Imagens
# Criar uma imagem a partir de um Dockerfile
docker build -t <image_name>:<tag> .

# Forçar rebuild sem cache
docker build --no-cache -t <image_name>:<tag> .

########## Gerenciar Imagens ##########
# Listar imagens locais
docker images

# Remover uma imagem local
docker rmi <image_id>

# Baixar uma imagem do Docker Hub
docker pull <image_name>

########## Manipular Volumes ##########
# Criar um volume
docker volume create <volume_name>

# Listar volumes
docker volume ls

# Remover um volume
docker volume rm <volume_name>

# Inspecionar um volume
docker volume inspect <volume_name>

########## Outros Comandos Úteis ##########
# Parar um container
docker stop <container_id>

# Iniciar um container parado
docker start <container_id>

# Remover um container
docker rm <container_id>

# Remover todos os containers parados
docker container prune
