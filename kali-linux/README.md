#Inicializar proyecto 

1-Crear imagen 

docker build -t kali-linux-docker . 

2-Crear Contenedor y ejecuta APP

docker run -it --rm --name kalilinux_container kali-linux-docker

docker run --rm -it -v ${PWD}/src:/usr/src/myapp --name kalilinux_container -i kali-linux-docker


3- Acceder a contenedor

docker exec -i -t kalilinux_container bash