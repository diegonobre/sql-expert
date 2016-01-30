Introdução ao SQL
==========
Neste guia utilizaremos os ícones abaixo para identificar em que plataforma/versão a instrução foi testada.

![](https://img.shields.io/badge/Oracle-9g-red.svg) ![](https://img.shields.io/badge/PostgreSQL-9.0-blue.svg) 

Nesta parte iremos conhecer a sintaxe SQL, aprender a criar estruturas e manter dados; vamos popular uma base de dados e consultar estes dados.

Para tirar proveito do que é descrito aqui, você deve possuir uma conexão a um banco de dados e deve saber como executar comandos.

# A linguagem
 - Os principais SGBDs da atualidade utilizam o SQL padrão ANSI. [Wikipedia](https://pt.wikipedia.org/wiki/SQL)
 - A linguagem é *case insensitive*, **não** diferencia maiúsculo e minúsculo, desde que o nome do objeto não esteja entre aspas "".
 - A maior parte dos comandos SQL é facilmente portável entre os diferentes SGBDs. Isso quer dizer que boa parte do que você vai aprender aqui pode ser utilizado em qualquer banco de dados que utilize a linguagem SQL.

# Sintaxe SQL
A estrutura sintática da linguagem SQL é composta por um conjunto de palavras-chave finalizados com um **;** ou com o fim da entrada de dados.

A seguir um exemplo de comandos SQL sintaticamente corretos:
```sql
SELECT * FROM pessoa;
UPDATE pessoa SET idade = 18;
INSERT INTO pessoa VALUES (3, 'Paulo Freire', 30);
```

Acima temos uma sequência de três comandos válidos.

# Identificadores
Por identificador, entende-se o "nome dado a um objeto". A linguagem SQL estabelece alguns critérios para a identificação de objetos e nem todos os bancos de dados possuem as mesmas regras.

Os identificadores possuem um tamanho limite. O SGBD poderá retornar uma exceção ou diminiur automaticamente o tamanho do nome de uma variável ou objeto.

|SGBD|Limite|
|-|-|
|PostgreSQL|64 caracteres|
|Oracle|30 caracteres|

Um identificador deve começar com letras ou "_" (underline) mas pode ser burlado com o uso de aspas duplas.

> Todos os comandos SQL são palavras-chave reservadas. Você não pode utilizar no nome dos seus objetos (tabelas, funções, triggers, variáveis), as intruções padrão SQL como: **SELECT, INSERT, UPDATE, DELETE, ALTER, TABLE**, etc...

Você pode utilizar as aspas duplas para criar variáveis com letras maiúsculas, espaços e caracteres especiais mas **isso não é recomendado**. Na verdade, é **recomendado não utilizar**.

```sql
SELECT * FROM pessoa;
SELECT * FROM "Pessoa";
SELECT * FROM "Nome da pessoa";
SELECT * FROM "123";
SELECT * FROM _123;
```

Todas as instruções acima são válidas.

# Comentários
Os comentários não possuem palavras-chave e não são identificados como parte do comando SQL; eles são tratados como se fosse espaços em branco. A linguagem SQL permite dois tipos de comentários:

 - Comentário em linha
 - Comentário em bloco

Exemplo de comentário em linha:
```sql
SELECT 'algum texto' -- comentário aqui
  FROM tabela;
```

Exemplo de comentário em bloco:
```sql
SELECT 'algum texto' /* comentário maior
com bastante texto
e quebra de linha */
  FROM tabela;
```

> Written with [StackEdit](https://stackedit.io/).