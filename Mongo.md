# Mongo

## Database (Bases de Datos)
```
show dbs
```
Ver bases de datos
```
use nombre_base_de_datos
```
Usar base de datos
```
db.dropDatabase()
```
Eliminar base de datos.
> _**Nota**_: Antes de ejecutar el comando previamente debemos habernos posicionado en la base de datos con **use <nombre_base_de_datos>**

## Autenticación
```
db.auth("usuario","contraseña");
```
Autenticar el usuario de la base de datos.
> Nota: Antes de ejecutar el comando de autenticación debe hacer _**use admin**_. Esto porque los usuarios que registro para la administración de la base de datos
## Colecctions (Colecciones)
```
show collections
```
ver collecions de una base de datos, previamente debo usar una base de datos.
```
db.nombre_collecion.remove({})
```
Vaciar los datos de la colección (Tener cuidado no se puede revertir)

## Documentos
```
db.nombre_coleccion.find()
```
Consultar todos los datos de la colección
```
db.nombre_coleccion.find(filtro)
```
Consultar todos los datos de la colección con un criterio de filtro
- filtro: esta compuesto de forma { campo : valor }
```
db.nombre_coleccion.delete({})
```
Eliminar uno o más valores  (Tener cuidado no se puede revertir)
- filtro: esta compuesto de forma { campo : valor }

```
db.nombre_coleccion.aggregate([ { $project: { "rootSize": { $sum: { $bsonSize: "$$ROOT" } } } } ])
```
Ver peso de los documentos
# Información en la base de datos (Backup)
```
mongoimport --db <nombre base de datos> --collection <nombre de la colección> --file <ruta del archivo> --jsonArray
```
Comando para cargar información en mongo desde un archivo json


```
mongoexport --db <nombre base de datos> --collection <nombre de la colección> --jsonArray --out <ruta donde se guardara el archivo> 
```
Comando para exportar información de la base de datos en un archivo json