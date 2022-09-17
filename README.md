# funcao-concat-manual-SQL
A função CONCAT() adiciona duas ou mais expressões juntas.



# ------------Funcoes-comuns-manual-SQL----------

# Função MySQL CONCAT()

[❮ Anterior](https://www.w3schools.com/sql/func_mysql_character_length.asp)[funções mysql ❮](https://www.w3schools.com/sql/sql_ref_mysql.asp)[Próxima ❯](https://www.w3schools.com/sql/func_mysql_concat_ws.asp)

### Exemplo

Adicione várias strings juntas:

SELECT CONCAT("SQL ", "Tutorial ", "is ", "fun!") AS ConcatenatedString;

**EXEMPLO 2**

extrai um mês e um ano de uma data em forma de **STRING**

**SELECT ***, **CONCAT** (**EXTRACT** (**MONTH FROM** date), '/', **EXTRACT** (**YEAR FROM** date) **AS** nome_da_nova_coluna **from **nome_tabela;



[Experimente você mesmo »](https://www.w3schools.com/sql/trymysql.asp?filename=trysql_func_mysql_concat)

------

## Definição e Uso

A função CONCAT() adiciona duas ou mais expressões juntas.

**Nota:** Veja também a função [CONCAT_WS().](https://www.w3schools.com/sql/func_mysql_concat_ws.asp)

## Sintaxe

CONCAT(*expression1*, *expression2*, *expression3*,...)

## Valores dos parâmetros

| Parameter                                     | Description                                                  |
| :-------------------------------------------- | :----------------------------------------------------------- |
| *expression1, expression2, expression3, etc.* | Required. The expressions to add together.                   |
|                                               | **Note:** If any of the expressions is a NULL value, it returns NULL |

## Detalhes técnicos

| Funciona em: | De MySQL 4.0 |
| :----------- | ------------ |
|              |              |

------

## Mais exemplos

### Exemplo

Adicione três colunas em uma coluna "Endereço":

**SELECT CONCAT**(Address, " ", PostalCode, " ", City) **AS** Address
**FROM** Customers;
