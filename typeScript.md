# Typescript
> En este caso se usa **npx** para ejecutar la libreria de typescript y no tener que instalarla de forma global
```
npm install typescript --save-dev
```
Instalar ependencia para usar typescript

```
npx tsc --init
```
Crear el fichero dtsconfig.json son los valores por defecto que puede ser configurable
```
npx tsc archivo 
```
Ejecutar archivo
```
npx tsc archivo --wath
```
Ejecutar archivo y estar atento a los cambios, para volver a realizar el proceso de transpilación.
```
npx tsc archivo --target es6
```
--target es6: Esta es una opción del compilador de TypeScript que establece la versión de ECMAScript a la que se debe compilar el código.