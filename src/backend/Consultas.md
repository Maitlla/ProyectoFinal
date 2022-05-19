# **Consultas SQL**

# SQLITE

- Consultar la información de ciertas columnas de las tablas.

sqlite> SELECT Rental_id, Name, DNI, Email, Phone, Code_postal FROM Rental;

SELECT Rental_id, Name, DNI, Email, Phone, Code_postal FROM Rental;

SELECT Rental_articles_id, Articles_id, Quantity, Price, Method_of_payment FROM Rental_articles;

SELECT Price FROM Rental_articles WHERE rowid=5;

SELECT Price FROM Rental_articles WHERE Articles_id='5'

SELECT Name, Photo FROM Articles WHERE rowid=4;

SELECT Articles_id FROM Articles WHERE Name='Evolutiva' AND Category_id='20';

SELECT Articles_id FROM Articles WHERE Name='Evolutiva' OR Category_id='20';

SELECT * FROM Staff ORDER BY Email;

SELECT * FROM Staff ORDER BY Name, Active;

SELECT * FROM Staff WHERE Active='1' ORDER BY Name, DNI;

- Modifica información de ciertas columnas de las tablas.

-- Cam


- Eliminar información de ciertas columnas de las tablas.

-- Se elimina la fila de ese id

DELETE FROM Staff WHERE Staff_id = 4;

-- Elimina las Direciones especificadas.

DELETE FROM Staff WHERE Address = 'Rua Aldea, 4' OR Address = 'Plaza Mayor, 10';

-- Elimina toda la tabla.

DROP TABLE Staff;

- Función que añade una columna concreta a una tabla

export function insertColumn() {
    const sql =  
    `ALTER TABLE users
    ADD COLUMN email TEXT NOT NULL DEFAULT ""`;
    taskss.run(sql);
}

//insertColumn() comentado para que no se ejecute

- Función que elimina una columna concreta de una tabla

export function deleteColumn() {
    const sql =  
    `ALTER TABLE users
    DROP COLUMN email`;
    taskss.run(sql);
}

//deleteColumn()

# PostgreSQL

