# Inicializar proyecto 

# 1-Crear imagen 

  docker build -t openjdk8 . 

# 2-Crear Contenedor y ejecuta APP

  docker run -it --rm --name openjdk8_container openjdk8

  docker run --rm -it -v c:/docker/openjdk/openjdk8/src:/usr/src/myapp --name openjdk8_container -i openjdk8

# 3- Acceder a contenedor

  docker exec -i -t openjdk_container bash
