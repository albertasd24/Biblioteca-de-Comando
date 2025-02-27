# PostgreSQL
## 📌 Sentencias Básicas de SQL

### 🔹 Crear una Base de Datos
```sql
CREATE DATABASE nombre_base_datos;
```

### 🔹 Listar Bases de Datos
```sql
\l  -- Comando en psql para listar bases de datos
SELECT datname FROM pg_database; -- Consulta SQL para listar bases de datos
```

### 🔹 Conectarse a una Base de Datos
```sql
\c nombre_base_datos;  -- Comando en psql para conectarse a una base de datos
```

### 🔹 Eliminar una Base de Datos
```sql
DROP DATABASE nombre_base_datos;
```

### 🔹 Seleccionar Datos
```sql
SELECT * FROM nombre_tabla; -- Seleccionar todos los registros de una tabla
SELECT columna1, columna2 FROM nombre_tabla; -- Seleccionar columnas específicas
SELECT DISTINCT columna FROM nombre_tabla; -- Seleccionar valores únicos
SELECT * FROM nombre_tabla WHERE columna = 'valor'; -- Filtrar registros
```

### 🔹 Inserción de Datos
```sql
INSERT INTO nombre_tabla (columna1, columna2) VALUES ('valor1', 'valor2');
```

### 🔹 Actualización de Datos
```sql
UPDATE nombre_tabla SET columna1 = 'nuevo_valor' WHERE columna2 = 'condicion';
```

### 🔹 Eliminación de Datos
```sql
DELETE FROM nombre_tabla WHERE columna = 'valor';
```

### 🔹 Creación de Tablas
```sql
CREATE TABLE nombre_tabla (
    id SERIAL PRIMARY KEY,
    nombre VARCHAR(50),
    edad INT
);
```

### 🔹 Eliminación de Tablas
```sql
DROP TABLE nombre_tabla;
```

---

## 📌 PostgreSQL - Uso de Schemas

En PostgreSQL, un **schema** es un contenedor lógico que organiza las bases de datos, similar a un namespace.

### 🔹 Crear un Schema
```sql
CREATE SCHEMA schema_stiven;
```

### 🔹 Listar Schemas Existentes
```sql
SELECT schema_name FROM information_schema.schemata;
```

### 🔹 Renombrar un Schema
```sql
ALTER SCHEMA schema_stiven RENAME TO schema_new_stiven;
```

### 🔹 Eliminar un Schema y Todo su Contenido

```sql
\dt  -- Comando en psql para listar tablas
SELECT table_name FROM information_schema.tables WHERE table_schema = 'public'; -- Consulta SQL para listar tablas
```