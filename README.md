# BD
comandos &amp; exemplos de BD

# MENU BD :mag:
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>
- :pushpin: [Select](#comando-select) <br>

<br>
<br>
<br>

## :bookmark: Comando SELECT
O comando SELECT é utilizado para recuperar dados de um banco de dados em SQL 


<i>A instrução SQL a seguir seleciona TODAS as colunas da seção "Customers":</i>
```
SELECT * FROM Customers;
```

<i>A instrução SQL a seguir seleciona as colunas "CustomerName", "City" e "Country" da tabela "Customers":</i>
```
SELECT CustomerName, City, Country FROM Customers;
```

<i>A instrução SELECT DISTINCT é usada para retornar apenas valores distintos (diferentes). Dentro de uma tabela, uma coluna geralmente contém muitos valores duplicados, e às vezes você deseja apenas listar os valores diferentes (distintos).
A instrução SQL a seguir seleciona apenas os valores DISTINCT (distintos) da coluna "Country", na tabela "Customers":</i>
```
SELECT DISTINCT Country FROM Customers;
```

A instrução SQL a seguir conta e retorna o número de países diferentes (distintos) na tabela "Customers":
```
SELECT COUNT(DISTINCT Country) FROM Customers;
```

<br>
<br>
<br>

## :bookmark: Comando UPDATE
## :bookmark: Comando DELETE
## :bookmark: Comando INSERT INTO
## :bookmark: Comando CREATE DATABASE
## :bookmark: Comando ALTER DATABASE
## :bookmark: Comando CREATE TABLE
## :bookmark: Comando ALTER TABE
## :bookmark: Comando DROP TABLE
## :bookmark: Comando CREATE INDEX
## :bookmark: Comando DROP INDEX
