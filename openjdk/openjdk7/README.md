#Inicializar proyecto 

1-Crear imagen 

docker build -t openjdk . 

2-Crear Contenedor y ejecuta APP

docker run -it --rm --name openjdk_container openjdk

docker run -it rm --name openjdk_container openjdk

docker run --rm -it -v c:/docker/openjdk/src:/usr/src/myapp --name openjdk_container1 -i openjdk

C:\docker\openjdk\src

3- Acceder a contenedor

docker exec -i -t openjdk_container bash