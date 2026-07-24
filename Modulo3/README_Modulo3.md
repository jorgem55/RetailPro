# Ventas_Tech_DB - Entrega Modulo 3 - Jorge Martinez
Script SQL que crea la base de datos ventas_Tech_Db para control de ventas de TechStore

## Contenido ventas_tech_db.sql
1. DDL, creación de las tablas (Categorias, Clientes, Productos, Ventas)
2. CONSTRAINT, PRIMARY KEY, FOREIGN KEY y NOT NULL en campos críticos.
3. DML, carga inicial de datos: 3 categorías, 3 clientes, 5 productos y 10 ventas.
4. Una consulta de validación con JOIN que devuelve las filas/ventas, combinando datos de las 4 tablas.
También incluye sentencias DROP TABLE IF EXISTS en orden inverso de dependencias para que el script sea repetible.

## Relaciones de atributos del modelado de datos
- Productos.CategoriaID --> Categorias.CategoriaID
- Ventas.ProductoID --> Productos.ProductoID
- Ventas.ClienteID --> Clientes.ClienteID

## Notas
- Los precios usan DECIMAL(10,2) en lugar de FLOAT, para evitar imprecisiones en cálculos monetarios (SUM, AVG, etc.).
- Las categorías están en tabla separada para cumplir la Tercera Forma Normal (3NF).

## Conclusión
En esta 3era entrega aplicamos los conceptos aprendidos sobre el diseño y creación de base de datos relacionales, a través de script SQL y utilizando repositorio de GitHub.