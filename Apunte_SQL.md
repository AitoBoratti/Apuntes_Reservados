# APUNTE DE SQL

SQL (Structured Query Language) es un lenguaje usado para manejar bases de datos relacionales. Te permite:
  * Almacenar datos de forma estructurada.
  * Consultar información rápidamente.
  * Actualizar y eliminar datos.

Ejemplo de bases de datos comunes que usan SQL:
  * SQLite (ligera, ideal para aprender).
  * MySQL (muy usada en desarrollo web).
  * PostgreSQL (avanzada y robusta).

Nota: Por convencion, los comandos van en mayusculas, y todas las lineas con punto y coma.
## Comandos basicos

CREATE TABLE "tu_tabla"; = Sirve para crear una tabla con el nombre elegido. A su vez, esta suele ir 
                           acompañada de un parentesis donde modificar datos.
CREATE TABLE "tu tabla"(
 -- "nombre" "t-dato" "propiedades" =  Esta es la forma de crear una columna, donde se pueden colocar variedad
                                    -- de propiedades utiles.
    id int PRIMARY KEY AUTO_INCREMENT,    -- Aqui se puede ver claramente propiedades como primary key, que indica 
                                          -- que esta sera la columna que sirva para identificar, o auto increment,
                                          -- que incrementa autimaticamente el valor
);
