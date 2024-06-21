En base a las tablas del diagrama adjunto, generar las siguientes consultas usando las sentencias vistas en clase.


- Contar el número de productos de una categoría específica.

```
SELECT COUNT(*) AS num_productos
FROM product
WHERE category = 'Electronics';

```

![[Pasted image 20240603162749.png]]

- Contar el número de clientes en una ciudad específica.

```
SELECT COUNT(*) AS num_clientes
FROM client
WHERE city = 'New York';

```

![[Pasted image 20240603162845.png]]

- Contar el número de productos cuyo precio está dentro de un rango específico

```
SELECT COUNT(*) AS num_productos
FROM product
WHERE price BETWEEN 100 AND 500;

```

![[Pasted image 20240603162938.png]]

- Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico

```
SELECT *
FROM client
WHERE city = 'Chicago' AND type_of_client = 'Regular';

```

![[Pasted image 20240603163025.png]]

- Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico

```
SELECT *
FROM product
WHERE category = 'Electronics' AND price > 500;


```

![[Pasted image 20240603163105.png]]


- Seleccionar productos que fueron producidos en un año específico y en un país de origen específico

```
SELECT *
FROM product
WHERE year_of_production = '2020' AND country_of_origin = 'China';


```

![[Pasted image 20240603191623.png]]

- Seleccionar clientes cuyo nombre completo comience con 'J'.

```
SELECT *
FROM client
WHERE fullname LIKE 'J%';

```

![[Pasted image 20240603191730.png]]

- Seleccionar clientes cuya ciudad contenga la letra 'a'

```
SELECT *
FROM client
WHERE city LIKE '%a%';

```

![[Pasted image 20240603191849.png]]