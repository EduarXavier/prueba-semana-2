# prueba-semana-2

# DOCKER

- Paso 1 y 2- creación del arhivo Dockerfile:

![Dockerfile-punto1](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/898d83f4-6eb6-43f5-92a5-b26bd26648df)

- Segundo paso - creación de la imagen y configuración de nginx:

![creacion-imagen-punto-1](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/27f90078-a841-4bea-a193-66a342514e4b)

![config-nginx-punto-1](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/91be9b6b-1c42-49ba-a757-682fac5f5fd1)

- Tercer paso - Creación de un contenedor partiendo de la imagen creada:

![creacion-contenedor-punto-1](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/5aff2d0b-ee4b-4e25-9c2a-188f19b8c229)

- Verificación del contenedor corriendo:

![contenedor-ejecutandose](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/55b0c11b-c9d6-469b-bac2-4c581f6d273c)

- Ingreso al contenedor:
  
![Ingreso al contenedor](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/4d9a6060-5267-4dbb-968c-2e71c11c1d24)

- Verificación de la funcionalidad:

![muestra-pagina-punto-1](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/a1ec5d01-1327-4165-97e7-e09a4ae18785)

- Estructura de las carpetas:

![tree punto 1](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/838e2329-4642-4d38-8b5f-8fde3178475f)


# Docker-compose y Docker-swarm

- Paso 1 y 2 - creación del dockerfile que se ejecuta a partir de la imagen de node, copia los archivos del api, instala sus dependencias y ejecuta el server.

![paso1-dockerfile](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/6302bb19-f67c-4818-a9c5-bba1e8354df7)

- - Construcción de la imagen:

![paso1-creacion-imagen](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/9bed4687-6886-40a0-ac37-c1243801eb97)


- - Verificación del dockerfile corriendo un contenedor que se elimina cuando este se detiene partiendo de esa imagen, mapeando el puero 8080 del anfitrion al 8080 del contenedor y estableciendo una variable de entorno:

![paso1-corrieno-contenedor](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/53e75fc3-ee08-42e9-b422-4cda070e3b6b)

- - Verificación de la variable de entorno:

![paso1-verificacion-variable](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/8bcb8efd-64eb-4634-8063-4066348c8a5e)

- - Estructura de las carpetas:

![paso1-estructura](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/bcd673ab-def0-43ed-b966-f39732134421)

- - Comprobación del api:

![paso1-comprobación-api](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/40f09706-b966-4811-a4cf-074b9b5e2f4d)

- Paso 3 y 4:

- - Docker-compose.yml con la red tipo bridge conectando los contenedores e implementación de los volumenes

![paso3-docker-compose](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/ebae1adf-a993-42bc-98e7-5a35179dff04)

- - Creación de los contenedores

![paso3-4-contenedores-corriendo red](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/f3052c60-9b4e-4bb5-be13-db1e41db6304)


- - Estructuración de las capetas:

![paso3-estructura](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/8f5a049c-426f-4593-b8d0-e278ff4b5f44)

- - creación de los certificados:

![paso3-creacion-certificado](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/3b0e63df-ba68-42ee-a612-ed73e7d6a8d1)


- -Ingreso al servicio de nginx desde la navegación https con certificados autofirmados funcionando como proxy inverso:

![certificado-paso-3](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/08d69566-87bd-43f4-87e2-bd880390b1cf)


- - Ingreso desde el servicio del api por http al puerto 8080.

![paso3-accediendo-desde-conteendor-api](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/707ba964-1c9b-4091-a911-bb8bd8146163)

-- Entrando a la bd con la clave que se ingresó en secretos:

![paso3-conteendor-bd-con-clave-secretos](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/8b257140-ab0a-466f-a2da-28901b3a16bf)


- Paso 5:

- - Ingreso de datos a la base de datos:

![Punto5-insertar-datos](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/7c9d0875-9d4c-4be5-abb4-a93cf9d77f05)

![punto5-insert-user](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/82907358-caf7-4780-b480-472041c5b9c7)


- - Detención de contenedores:
![paso5-detencionn-de-conteendores](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/8e0ef4f8-3243-4661-9b5e-af7ae8f4598c)

- - Verificación de la persistencia de datos:

![punto5-peristencia-datos](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/808b38a2-dbb1-4a1b-aeb5-0bd80b017245)


- Punto 6

- -- Estructura de carpetas:

![punto6-estructura](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/00d6f6de-4bf1-4e57-ba35-f8bc2d51964b)


- - Pasar de docker-compose a docker-swarm:

![punto6-docker-stack](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/63af9858-5ff7-4f44-84c8-1a75ec306454)

- - Inicialización del nodo:

![paso6-creacion-nodo-manager](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/ff562218-a052-42c2-9853-41d72f613ace)

- - Verificación del nodo:

![punto6-nodo](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/ba8622b5-7a9c-4f47-920b-6901a7941150)

- - Deploy de los servicios

![punto-6-deploy](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/fd970934-b7e2-496e-b3b7-449b1ab89c50)

- - Verificación de los conteendores corriendo:

![punto6-contenedores](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/f3e8501c-5ea2-4f65-8a64-cd831c5cedec)

- - Verificación de los servicios 

![punto6-servicios](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/108fd854-bed9-48fa-b57b-afc85ed46b15)


- - Ver donde está corriendo un servicio:

![punto-6-ver-corriendo-api](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/c3000a69-ba6d-4d73-823a-fd980fcbbd67)

- - Verificación del balanceo de carga en los servicios (Node no da logs debido a que no se estableció en el api):

![paso6-logs](https://github.com/EduarXavier/prueba-semana-2/assets/142350836/c7e9df92-1508-4844-85be-0fcfe5038a94)

-- Realizado por: Eduar Xavier Avendaño --


