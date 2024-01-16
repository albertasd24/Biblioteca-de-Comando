# Python

## Entorno Virtual
> Un entorno virtual en Python es como un espacio independiente que encapsula las herramientas y bibliotecas necesarias para un proyecto específico, sin afectar a otros proyectos que puedas tener en tu sistema. Esto facilita la gestión de dependencias y versiones en entornos de desarrollo.

### Windows
```
python -m venv nombre_entorno_virtual
```
Crear un entorno virtual

```
nombre_carpeta_entorno\Scripts\activate
```
Activar entorno virtual

```
deactivate
```
Desactivar entorno virtual

## pip (Gestor de dependencias)
> Pip es el administrador de paquetes, quiere decir que es el que nos permite instalar librerias al proyecto. Tal como lo es npm en javascript y maven/Grandle en java
```
pip install nombre_libreria
```
Instala la libreria que se haya indicado
```
pip install nombre_libreria==número_versión
```
Instala la libreria con una versión en específico
```
pip install -r requirements.txt
```
Instala las librerias que se encuentren registradas en el archivo requirements.txt
```
pip list
```
Lista las librrias instaladas en un proyecto
