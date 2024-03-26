# Busquedas condicionales

## Busquedas 
_selecciona todos los documentos de una coleccion_

```m

db.libros.find()
db.libros.find({})

```

_seleccionar todos los documentos de la coleccion libros donde la editorial sea Biblio_

```m
db.libros.find
({editorial:'biblio'})
```

_seleccionar todos los documentos de la coleccion libros donde el precio sea igual a 25_

```m
db.libros.find(
... {precio:25})
```

## Busquedas con operadores logicos

**Sintaxis**
```m
{<columna>:
{<operador>:<valor>}, ...}
```

_seleccionar todos aquellos documentos de la coleccion libros donde el recio sea mayor a 25_

```m
db.libros.find({precio:{$gt:25}})
```