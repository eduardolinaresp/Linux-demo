# Inicializar proyecto 

## 1-Crear imagen 

     ##docker build -t centos7_images .
	 docker build --rm -t local/c7-systemd .

## 2-Crear Contenedor en powerShell or Linux.

   	
	docker run --rm -d -v ${PWD}/src:/usr/AngularTest/src -p 8080:8080 --name centos7_container -i centos7_images

  
    _Nota: Debido a Firewall de windows expongo mi localhost:80_

## 3 - Filtros Sobre Procesos Docker 

    docker ps -a -q --filter="name=centos7_container" 


## 4- Acceder a contenedor

    docker exec -it -t centos7_container /bin/sh


## 5- Detener  contenedor

    docker stop centos7_container


    

