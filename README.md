# postgre-syntax

docker exec -it postgres psql -U postgres

\l untuk melihat list

\c untuk masuk kedalam table

\dt utnuk meliat list table dalam database

CREATE TABLE nama_table (id serial primary key not null, name varchar(100), price float, stock int);

INSERT INTO products (id, product_name, product_price, product_stock) VALUES (3, 'Mie Sedap', 2000, 20);

UPDATE products SET product_name='Indomie Bawang' WHERE id = 1;

UPDATE products SET product_stock=40 WHERE id IN(2,3);

DELETE FROM products WHERE id = 1;

DELETE FROM products WHERE id IN(1,2);

ALTER TABLE products RENAME COLUMN product_name to name;
