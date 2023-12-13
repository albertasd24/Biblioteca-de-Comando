# Docker

## Containers (Contenedores)
```
Docker ps
```
Ver contenedores corriendo
```
Docker ps -a
```
Ver todos los contenedores esten corriendo o no
```
Docker start nombre_contenedor/id_contenedor 
```
Iniciar Contenedor (ponerlo a correr)
```
Docker stop nombre_contenedor/id_contenedor
```
Detener un contenedor
```
Docker rm nombre_contenedor/id_contenedor
```
Eliminar un contenedor
```
Docker logs nombre_contenedor/id_contenedor
```
ver logs del contenedor
```
docker cp nombre_archivo nombre_contenedor:/ubicacion_a_enviar 
```
Enviar archivos del sistema a un contenedor
### Conectar a un contenedor
```
docker exec -it nombre_contenedor bash
```

# Images (Imagenes)
```
Docker images
```
Ver imagenes

# Volumes (Volumenes)
```
Docker volume ls
```
Ver volumenes creados
```
docker volume inspect avatar_files
```
Ver información detalle de un volumen
# Docker-compose
```
docker-compose up --build -d
```
Construir un contenedor a partir de un archivo docker-compose

```
docker-compose dowm
```
Detener y bajas los contenedores con base en lo configurado al archivo docker-compose