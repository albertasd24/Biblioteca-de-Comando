# SSH

```
ssh-keygen -t rsa -b 4096 -C "correo"
```
Crear llave ssh
- t Definición de protocolo 
- b Definición de cantidad de complejidad del algoritmo 

```
eval $(ssh-agent -s)
```
Confirmar que el servicio de llaves este activo