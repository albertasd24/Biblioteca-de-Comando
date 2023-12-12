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
db.nombre_collecion.delete({})
```
Eliminar uno o más valores  (Tener cuidado no se puede revertir)
- filtro: esta compuesto de forma { campo : valor }

# Información en la base de datos (Backup)
```
mongoimport --db <nombre base de datos> --collection <nombre de la colección> --file <ruta del archivo> --jsonArray
```
Comando para cargar información en mongo desde un archivo json


```
mongoexport --db <nombre base de datos> --collection <nombre de la colección> --jsonArray --out <ruta donde se guardara el archivo> 
```
Comando para exportar información de la base de datos en un archivo json