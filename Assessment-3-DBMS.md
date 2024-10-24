
``` SQL

create table products (pro_id(4), pro_name varchar(40), pro_price float,pro_code int (4));

insert into products values
(101, "Mother Board", 3200.00, 15),
(102, "key Board", 450.00, 16),
(103," ZIP drive", 250.00, 14),
(104, "Speaker", 550.00, 16),
(105, "Monitor", 5000.00, 11),
(106, "DVD drive", 900.00, 12),
(107, "CD drive", 800.00, 12),
(108, "Printer", 2600.00, 13),
(109, "Refill cartridge", 350.00, 13),
(110, "Mouse", 250.00, 12);

SELECT pro_name, pro_price FROM products WHERE pro_price >= 250
ORDER BY  pro_price desc, pro_name asc;

SELECT pro_name, pro_price FROM products ORDER BY pro_price asc limit 1;

SELECT AVG(pro_price) AS average_price from products;

SELECT sum(pro_price) AS Total_price from products;
```