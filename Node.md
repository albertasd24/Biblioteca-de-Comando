# Node.js
> Nodejs es un entorno de ejecución para javascript, su objetivo es poder sacar el motor de javascript del navageador y llevarlo a servidor y equipos locales. 

```
node
```
El comando anterior llama al interprete en la terminal

## NPM (Node Package Manage)
> Npm es el administrador de paquetes de javascript, se encargar de proporcionar la facilidad para instalar libreriar al proyecto. Tal como lo es npm en javascript y maven/Grandle en java

### Iniciar un nuevo proyecto con Node js
```
npm init
```
Inicia un nuevo proyecto Node.js. Este comando guía al usuario a través de la creación de un archivo package.json interactivo. Para omitir las preguntas de configuración del proyecto añadir la banderita -y
#
```
npm list
```
Muestra la lista de todos los paquetes/librerias instalados en el proyecto

```
npm info nombre_del_paquete
```
Muestra información detallada sobre un paquete
```
npm run nombre-del-script
```
Ejecuta un script definido en el archivo **package.json**
```
npm update
```
Actualiza los paquetes a las versiones más recientes, según las restricciones definidas en el archivo package.json.
```
npm search nombre_del_paquete
```
Busca paquetes en el registro de npm.