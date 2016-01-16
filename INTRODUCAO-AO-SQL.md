Introdução ao SQL
==========
Neste guia utilizaremos os ícones abaixo para identificar em que plataforma/versão a instrução foi testada.

![](https://img.shields.io/badge/Oracle-9g-red.svg) ![](https://img.shields.io/badge/PostgreSQL-9.0-blue.svg) ![](https://img.shields.io/badge/MySQL-5.0-green.svg) ![](https://img.shields.io/badge/SQLServer-2010-yellow.svg)

# A linguagem
 - Os principais SGBDs da atualidade utilizam o SQL padrão ANSI. [Wikipedia](https://pt.wikipedia.org/wiki/SQL)
 - A linguagem é *case insensitive*, **não** diferencia maiúsculo e minúsculo, desde que o nome do objeto não esteja entre aspas "".
 - A maior parte dos comandos SQL é facilmente portável entre os diferentes SGBDs. Isso quer dizer que boa parte do que você vai aprender aqui pode ser utilizado em qualquer banco de dados que utilize a linguagem SQL.

> Todos os comandos SQL são palavras-chave reservadas. Você não pode utilizar no nome dos seus objetos (tabelas, funções, triggers, variáveis), as intruções padrão SQL como: SELECT, INSERT, UPDATE, DELETE, ALTER, TABLE, etc...

Você pode utilizar as aspas duplas para criar variáveis com letras maiúsculas, espaços e caracteres especiais mas **isso não é recomendado**. Na verdade, é **recomendado não utilizar**.

```sql
SELECT * FROM pessoa;
SELECT * FROM "Pessoa";
SELECT * FROM "Nome da pessoa";
```

Todas as instruções acima são válidas.



> Written with [StackEdit](https://stackedit.io/).