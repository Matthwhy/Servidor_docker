# Servidor_docker
Um servidor criado a base de docker


https://github.com/Matthwhy/Servidor_docker.git

#Entrar na pasta do código#

cd 03_Dockerfile

#constuir imagens Docker a partir de um Dockerfile#

docker build -t=hello_flask .

#Imagem criada#

docker image ls

#rodar imagem#
docker run hello_flask &
docker stop

#Rodar servidor e fazer conexão interna e externa#

docker run -p 4000:80 --name app_hello hello_flask &

#Parar servidor#
docker stop app_hello
