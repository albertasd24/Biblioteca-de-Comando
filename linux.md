# Linux
> Nota estos comandos sirven en cualquier distribución de Linux, o sea Ubuntu, debian, kali linux, etc.

- [Comandos Básicos Linux](#comandos-básicos)
- [Nano](#comandos-básicos)
## Comandos Básicos:
```
pwd
```

Muestra el directorio de trabajo actual.
```
ls
```

Lista archivos y directorios en el directorio actual.
```
cd
```
Cambia el directorio de trabajo.
```Ejemplo: cd carpeta```
```
cp
```

Copia archivos o directorios.
```Ejemplo: cp archivo.txt destino/```
```
mv
```

Mueve o renombra archivos o directorios.
```Ejemplo: mv archivo.txt nuevo_nombre.txt```

```
rm
```

Elimina archivos o directorios.
```Ejemplo: rm archivo.txt```

```
mkdir
```

Crea un nuevo directorio.
```Ejemplo: mkdir nuevo_directorio```

```
rmdir
```
Elimina un directorio vacío.
```Ejemplo: rmdir directorio_a_eliminar```

## Comandos de Visualización y Búsqueda:
```
cat
```
Muestra el contenido de un archivo.
```Ejemplo: cat archivo.txt```
```
more
```

Muestra el contenido de un archivo de manera paginada.
```Ejemplo: more archivo.txt```

```
less
```

Similar a more, pero permite navegar hacia atrás.
```Ejemplo: less archivo.txt```

```
grep
```

Busca patrones en archivos.
```Ejemplo: grep "patron" archivo.txt```

## Comandos de Administración del Sistema:
```
ps
```
Muestra procesos en ejecución.
```Ejemplo: ps aux```
```
top
```
Muestra una lista en tiempo real de los procesos en ejecución.
```
kill
```

Termina un proceso.
```Ejemplo: kill PID```

```
chmod
```

Cambia los permisos de un archivo o directorio.
```Ejemplo: chmod 755 archivo```

```
chown
```
Cambia el propietario de un archivo o directorio.
```Ejemplo: chown usuario:grupo archivo```
```
df
```
Muestra el espacio en disco utilizado y disponible.
```
du
```
Muestra el espacio en disco utilizado por archivos y directorios.
```Ejemplo: du -h directorio```

## Archivos
```
touch nombre_archivo
```
Crear un archivo. ```Ejemplo: touch nombreArchivo.extensión```


### mv tiene dos funcionalidades
```
mv archivo ubicacion_a_enviar
```
Mover un archivo o carpeta.```Ejemplo: mv imagen.jpg carpeta_imagenes/```
```
mv nombre_antinuo nombre_nuevo
```
Cambiar el nombre de un archivo. ```Ejemplo: mv imagenCat.jpg imagenGato.jpg```
### Comprimir y descromprimir

```
tar -czvf carpeta/archivo
```
Comprimir carpeta/archivo. ```Ejemplo: tar -czvf carpeta archivo```
```
tar -zxf carpeta_comprimida
```
Descromprimir carpeta.```Ejemplo: tar -zxf carpeta_comprimida```

## Nano
Abrir un archivo:

```
nano nombre_archivo.txt
```
Abre o crea el archivo nombre_archivo.txt en Nano.

Guardar Cambios:
```
Ctrl + O
Ctrl + s
```
Salir de Nano:
```
Ctrl + X
```
Cierra Nano. Si hay cambios sin guardar, te preguntará si deseas guardar antes de salir.

Buscar Texto:
```
Ctrl + w
```
Abre la opción de búsqueda. Ingresa el texto a buscar y presiona Enter.

Cortar Texto:
```
Ctrl + k
```

Pegar Texto:
```
Ctrl + U
```
Pega el texto previamente cortado en la posición del cursor.

Moverse hacia arriba o abajo
```
Ctrl + ↑ (Flecha arriba) / Ctrl + ↓ (Flecha abajo)
```
Mueve el cursor hacia arriba o abajo en el archivo.

Ir al inicio o al final del archivo:
```
Ctrl + ↑ (Flecha izquierda) / Ctrl + ↓ (Flecha derecha)
```
Mueve el cursor al principio o al final de la línea actual.

Mostrar información de la línea y columna:
```
Ctrl + C
```
Muestra la posición actual del cursor.