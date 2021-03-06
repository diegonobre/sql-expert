# Projeto de Banco de Dados

Este capítulo pretende introduzir o leitor nos conceitos de modelagem conceitual e relacional de bancos de dados. Aqueles que já possuem experiência com no tema podem aproveitar para revisar alguns conceitos ou avançar para o próximo capítulo.

Segundo Heuser (1998), um projeto de banco de dados envolve duas fases:

1. Modelagem Conceitual
  > Captura as necessidades da organização quanto ao armazenamento de dados independente da implementação.

2. Modelagem Lógica
  > Transforma o modelo conceitual em modelo lógico definindo como o banco de dados será implementado em um SGBD específico.

Em artigo publicado em 2011 entitulado "Persistência Poliglota" ¹, Martin Fowler apresenta uma perspectiva ampla quanto ao tipo de persitência de dados que pode ser utilizada associada a um software.

A imagem a seguir apresenta o tipo de persistência dependendo do tipo de dado que está sendo manipulado [origem da imagem](http://martinfowler.com/bliki/images/polyglotPersistence/polyglot.png)
![Speculative Retailers Web Application](img/martin_fowler_polyglot_persistence.png)

Muito tem se falado sobre os bancos de dados não relacionais (noSQL). O uso do MongoDB é altamente recomendado para grandes massas de dados que recebem milhares de acessos simultâneos. Não iremos nos aprofundar no conceito de banco não relacional já que o nosso foco aqui é o SQL.

Ao iniciar um projeto de software, diferentes metodologias são aplicadas. Quando a escolha da plataforma de persistência é o banco de dados relacional, uma etapa crucial antes de iniciar o desenvolvimento da aplicação é a elaboração do `Projeto de Banco de Dados`.

O projeto de banco de dados, de acordo com a disponibilidade de tempo e recursos da equipe, pode envolver a criação de `modelos conceituais` e `modelos relacionais` do banco de dados

¹ "Polyglot Persistence" - http://martinfowler.com/bliki/PolyglotPersistence.html. Acessado em 30/01/2016.