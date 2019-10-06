
# SQL - Data Definition Language

## Conceitos

- Linguagem de Definição de Dados, define a estrutura dos dados e tabelas. Os comandos DDL mais comuns são CREATE, ALTER, DROP, RENAME e TRUNCATE;
- **CREATE:** Comando utilizado para criar um BANCO (CREATE DB) e uma TABELA (CREATE TABLE);
- **ALTER TABLE:** Comando usado para adicionar, excluir ou modificar as colunas de uma tabela existente;
- **DROP:** Comando utilizado para excluir dados. O DROP pode ser utilizado de três formas:
  * **DROP INDEX:** Exluir um indice em uma tabela;
  * **DROP TABLE:** Excluir uma tabela;
  * **DROP DATABASE:** Excluir um banco de dados.
- **RENAME:** Comando utilizado para renomear tabelas;
- **TRUNCATE:** Comando para excluir os dados de uma tabela, e não a tabela em si;


## Tipos de Dados
- Numéricos:
  * Integer Numbers: *INTEGER, INT, SMALLINT*;
  * Floating-point: *FLOAT, REAL, DOUBLE PRECISION*.
- Cadeia de caracteres:
  * Comprimento fixo: *CHAR(n), CHARACTER(n)*;
  * Comprimento variável: *VARCHAR(n), CHAR VARYING(n). CHARACTER VARYING(n)*.
- Bit-String:
  * Comprimento fixo: *BIT(n)*;
  * Comprimento variável: *BIT VARYING(n)*.
- Boolean:
  * Valores: *TRUE, FALSE ou NULL*.
- Date:
  * Componentes são *YEAR, MONTH, DAY* na forma de *YYYY-MM-DD*;
  * SGBDs fornecem diversos recursos para conversão de formato e manipulação de datas.

## Constraints
- SQL inclui 3 constraints básicas do modelo relacional:
  * **Integridade de chave:** Definidas com chaves primárias(**PRIMARY KEY**) - não podem ter valor duplicado em um atributo pertencente à tabela;
  * **Integridade de entidade:** Definidas com chaves primárias(**PRIMARY KEY**) - não podem ter valor *null* ou vazio;
  * **Integridade referencial:** Definidas com chaves estrangeiras(**FOREIGN KEY**) - devem conter um valor existente na tabela referenciada (mesmo que seja *null*).
