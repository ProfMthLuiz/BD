# BD
comandos &amp; exemplos de BD

# MENU BD :mag:
- :round_pushpin: [Select](#anchor-comando-select) <br>
- :round_pushpin: [Where](#anchor-comando-where) <br>
- :round_pushpin: [Update](#anchor-comando-update) <br>
- :round_pushpin: [Delete](#anchor-comando-delete) <br>
- :round_pushpin: [Insert Into](#anchor-comando-insert-into) <br>
- :round_pushpin: [Create Database](#anchor-comando-create-database) <br>
- :round_pushpin: [Alter Database](#anchor-comando-alter-database) <br>
- :round_pushpin: [Create Table](#anchor-comando-create-table) <br>
- :round_pushpin: [Alter Table](#anchor-comando-alter-table) <br>
- :round_pushpin: [Drop Table](#anchor-comando-drop-table) <br>
- :round_pushpin: [Create Index](#anchor-comando-create-index) <br>
- :round_pushpin: [Drop Index](#anchor-comando-drop-index) <br>

<br>
<br>
<br>

## :anchor: Comando SELECT
O comando SELECT é utilizado para recuperar dados de um banco de dados em SQL 


:paperclip: <i>A instrução SQL a seguir seleciona TODAS as colunas da seção "Customers":</i>
```
SELECT * FROM Customers;
```

:paperclip: <i>A instrução SQL a seguir seleciona as colunas "CustomerName", "City" e "Country" da tabela "Customers":</i>
```
 SELECT CustomerName, City, Country FROM Customers;
```

:paperclip: <i>A instrução SELECT DISTINCT é usada para retornar apenas valores distintos (diferentes). Dentro de uma tabela, uma coluna geralmente contém muitos valores duplicados, e às vezes você deseja apenas listar os valores diferentes (distintos). <br>
A instrução SQL a seguir seleciona apenas os valores DISTINCT (distintos) da coluna "Country", na tabela "Customers":</i>
```
SELECT DISTINCT Country FROM Customers;
```

:paperclip: A instrução SQL a seguir conta e retorna o número de países diferentes (distintos) na tabela "Customers":
```
SELECT COUNT(DISTINCT Country) FROM Customers;
```

<br>
<br>
<br>

## :anchor: Comando WHERE
É uma cláusula opcional que permite filtrar os resultados com base em uma condição específica.

:paperclip: <i>A instrução SQL a seguir seleciona TODOS os "Customers" do "Mexico":</i>
```
SELECT * FROM Customers WHERE Country = 'Mexico';
```

:paperclip: O MySQL requer aspas simples em torno de valores de texto (a maioria dos sistemas de banco de dados também permite aspas duplas). No entanto, os campos numéricos não devem ser colocados entre aspas. <br>
<i>A instrução SQL a seguir seleciona TODOS os "Customers" cujo o "CustomerID" seja 1:</i>
```
SELECT * FROM Customers WHERE CustomerID = 1;
```

<b> Os seguintes operadores podem ser usados ​​na cláusula WHERE: </b>

<i> <strong>(=) - </strong> Igual </i> <br>
<i> <strong>(>) - </strong> Maior que </i> <br>
<i> <strong>(<) - </strong> Menor que </i> <br>
<i> <strong>(>=) - </strong> Maior ou igual </i> <br>
<i> <strong>(<=) - </strong> Menor ou igual </i> <br>
<i> <strong>(<>) - </strong> Não é igual. Nota: Em algumas versões do SQL este operador pode ser escrito como (!=) </i> <br>
<i> <strong>(BETWEEN) - </strong> Usada para selecionar valores dentro de um intervalo específico. Pode ser usado com números, datas ou strings </i> <br>
<i> <strong>(LIKE) - </strong> É usada para buscar padrões em dados de texto. Ela é frequentemente utilizada com a wildcard %, que representa qualquer conjunto de caracteres. Existem duas principais wildcards usadas com LIKE: (%) Representa zero ou mais caracteres e _ (sublinhado) representa um único caractere. </i> <br>
<i> <strong>(IN) - </strong> É usada para comparar um valor a uma lista de valores. </i> <br>

<i> :pushpin: Exemplos de BETWEEN, LIKE & IN: </i>

:paperclip: <i>A instrução SQL a seguir seleciona produtos com preço entre 300 e 800:</i>
```
SELECT * FROM products WHERE price BETWEEN 300 AND 800;
```

:paperclip: <i>A instrução SQL a seguir seleciona produtos com nomes específicos:</i>
```
SELECT * FROM products WHERE product_name IN ('Laptop', 'Tablet', 'Camera');
```

:paperclip: <i>A instrução SQL a seguir seleciona produtos cujo nome começa com 'S':</i>
```
SELECT * FROM products WHERE product_name LIKE 'S%';
```

:paperclip: <i>A instrução SQL a seguir seleciona produtos cujo nome nome contém 'phone':</i>
```
SELECT * FROM products WHERE product_name LIKE '%phone%';
```

<br>
<strong>O comando WHERE, pode ser combinado com os OPERADORES AND, OR e NOT:</strong>
<br>
<br>

:pushpin:<i>WHERE com AND</i>
<br>

:paperclip: <i>A instrução SQL a seguir seleciona produtos com preço entre 100 e 500 E categoria é 'Electronics':</i>
```
SELECT * FROM products WHERE price BETWEEN 100 AND 500 AND category = 'Electronics';
```

<br>

:pushpin:<i>WHERE com OR</i>
<br>

:paperclip: <i>A instrução SQL a seguir seleciona produtos cujo 'price' é menor que 100 OU cuja 'category' é 'Accessories':</i>
```
SELECT * FROM products WHERE price < 100 OR category = 'Accessories';
```

<br>

:pushpin:<i>WHERE com NOT</i>
<br>

:paperclip: <i>A instrução SQL a seguir selecionaprodutos cujo price NÃO é maior que 200.:</i>
```
SELECT * FROM products WHERE NOT price > 200;
```
<br>

## :anchor: Comando UPDATE
## :anchor: Comando DELETE
## :anchor: Comando INSERT INTO
## :anchor: Comando CREATE DATABASE
## :anchor: Comando ALTER DATABASE
## :anchor: Comando CREATE TABLE
## :anchor: Comando ALTER TABLE
## :anchor: Comando DROP TABLE
## :anchor: Comando CREATE INDEX
## :anchor: Comando DROP INDEX
