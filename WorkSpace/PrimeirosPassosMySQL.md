# Primeiros Passos no MySQL

## Veja nesse artigo os principais comandos de SQL para se trabalhar com o banco de dados MySQL. Vamos aprender a criar um banco de dados e a criar, editar, buscar e excluir uma tabela no MySQL.

[Artigos](https://www.devmedia.com.br/artigos/)[Banco de Dados](https://www.devmedia.com.br/artigos/banco-de-dados)Primeiros Passos no MySQL

### Aprendendo a trabalhar com MySQL

Olá pessoal, no artigo de hoje vamos aprender a [trabalhar com o MySQL](https://www.devmedia.com.br/mysql-tutorial/33309), para um melhor entendimento, iremos aprender como fazer pelo terminal do **MySQL**, utilizando de código puro SQL.

Antes de qualquer coisa, vamos fazer o [download do MySQL](https://dev.mysql.com/downloads/) e vamos entender o que ele é.

**O MySQL é um sistema de gerenciamento de banco de dados (SGBD)**, que utiliza a [linguagem SQL](https://www.devmedia.com.br/entedendo-a-linguagem-sql/7775) (Structured Query Language ou Linguagem de Consulta Estruturada) como interface.

Saiba mais: [MySQL](https://www.devmedia.com.br/guia/mysql/34335)

**O MySQL atualmente é um dos maiores SGBD’s do mundo**, com mais de 10 milhões de instalações e vem sendo usado inclusive em projetos de grande porte em grandes empresas.

Entre essas empresas, estão: NASA, Friendster, Banco Bradesco, Dataprev, HP, Nokia, Sony, Lufthansa, U.S. Army, U.S. Federal Reserve Bank, Associated Press, Alcatel, Slashdot, Cisco Systems, Google, entre outros.

Não é a toa que **o MySQL cresceu tanto assim nos últimos anos**, abaixo segue uma lista de coisas que fizeram esse SGBD crescer tanto e continuar crescendo cada vez mais.

- Portabilidade (suporta praticamente qualquer plataforma atual);
- Compatibilidade (existem drivers ODBC, [JDBC](https://www.devmedia.com.br/curso/o-que-e-jdbc/1990) e .NET e módulos de interface para diversas linguagens de programação, como Delphi, Java, C/C++, C#, Visual Basic, Python, Perl, PHP,ASP e Ruby
- Excelente desempenho e estabilidade;
- Pouco exigente quanto a recursos de hardware;
- Facilidade de uso;
- É um Software Livre com base na GPL (entretanto, se o programa que acessar o Mysql não for GPL, uma licença comercial deverá ser adquirida);
- Contempla a utilização de vários Storage Engines como MyISAM, InnoDB, Falcon, BDB, Archive, Federated, CSV, Solid…
- Suporta controle transacional;
- Suporta Triggers;
- Suporta Cursors (Non-Scrollable e Non-Updatable);
- Suporta Stored Procedures e Functions;
- Replicação facilmente configurável;
- Interfaces gráficas (MySQL Toolkit) de fácil utilização cedidos pela MySQL Inc.

Agora vamos entender um pouco a sintaxe do mysql. Primeiro vamos ver como fazemos para criar um banco de dados pelo terminal do mysql.

### Criando o banco de dados

**Listagem 1**: Criando banco de dados



```
CREATE DATABASE bancodeteste;
```

Como podemos ver, a sintaxe é bem intuitiva e com um leve conhecimento da língua inglesa fica mais fácil ainda de entender.

Após criar o bando de dados, precisamos avisar ao mysql que vamos usá-lo, para isso basta escrevermos.

**Listagem 2**: Usando o banco de dados

```
USE bancodeteste;
```

Feito isso o nosso banco de dados está criado, faltando apenas criar a nossa tabela. Para isso vamos usar o comando CREATE TABLE.

### Criando tabelas

**Listagem 3**: Criando tabelas

```
CREATE TABLE fornecedores(
codigo int(4) AUTO_INCREMENT,
nome varchar(30) NOT NULL,
email varchar(50),
PRIMARY KEY (codigo)
);
```

Como podemos ver, nossa tabela está criada.

![Tabela criada](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL03-1.jpg)**Figura 1**: Tabela criada.

Agora vamos às explicações do que se tratam os comandos:

- AUTO_INCREMENT pode ser utilizado para automatizar um código que sirva de chave primária de uma tabela.
- PRIMARY KEY define a chave primária da tabela, isto é, o campo que serve como chave da tabela e que não pode ser repetido.
- NOT NULL define que um determinado campo seja de preenchimento obrigatório.

Agora já temos um banco de dados e uma tabela criada, com isso é possível manipular os dados do banco de dados.

### INSERT

Agora vamos inserir alguma informação na nossa tabela, para isso vamos usar o comando INSERT, é bem simples também.

**Listagem 4**: Inserindo Dados

```
INSERT INTO fornecedores(codigo, nome, email) VALUES (null, “Ricardo”, “ricoarrigoni@gmail.com”) ;
INSERT INTO fornecedores(codigo, nome, email) VALUES (null, “João”, “joao@gmail.com”) ;
INSERT INTO fornecedores(codigo, nome, email) VALUES (null, “Maria”, “maria@gmail.com”) ;
```

![ Dados inseridos na tabela](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL04-1.jpg)**Figura 2**: Dados inseridos na tabela.

### SELECT

Agora que nossa tabela está com alguns registros inseridos nela, nós vamos usar o comando SELECT pra poder selecionar e buscar esses registros. Continuaremos no mesmo terminal e iremos digitar o seguinte código:

**Listagem 5**: Usando o comando SELECT

```
SELECT * FROM fornecedores;
```

O Resultado desse SELECT nós vemos na Figura 5.

![Resultado do Select global](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL05.jpg)**Figura 5**: Resultado do SELECT global.

Como podemos perceber, todos os registros da tabela foram retornados. Isso se deu porque o uso do SELECT * faz com que a consulta retorne todos os valores da tabela.

Mas o comando SELECT permite diversas variações e combinações nele, podemos buscar exatamente o que queremos e do jeito que queremos, por exemplo.

Se quisermos buscar apenas o e-mail do fornecedor nós podemos, basta fazer da seguinte forma:

**Listagem 6**: Usando o SELECT específico

```
SELECT email FROM fornecedores;
```

Nesse caso ele irá exibir somente o que está no campo email do registro.

![Select específico](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL06.jpg)**Figura 3**: SELECT específico.

### ORDER BY

Se em nossa consulta sql nós quisermos que os registros retornados venham ordenados, nós podemos usar o comando ORDER BY, basta dizer pelo que você quer ordenar que ele traz o registro ordenado.

**Listagem 7**: SELECT usando ORDER BY

```
SELECT * FROM fornecedores ORDER BY nome asc;
```

Dessa forma, os registros retornados virão ordenados pelo campo nome em ordem alfabética. Mas como eu sei que virá em ordem alfabética?

Quando eu uso o termo “asc” eu digo que quero em ordem ascendente, se eu quiser fazer um SELECT que venha em ordem descendente, basta utilizarmos o “desc”.

O resultado da nossa busca pode ser visto aqui:

![Select ordenado por ordem alfabética](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL07.jpg)**Figura 4**: SELECT ordenado por ordem alfabética.

### UPDATE

Para alterar um registro, usamos o comando UPDATE, com ele é possível editar os campos de sua tabela e colocar outro valor neles.

**Listagem 8**: Editando registros

```
UPDATE fornecedores SET nome=”Ricardo Arrigoni” WHERE codigo=1;
```

Após esse comando, o nome “Ricardo” será alterado para “Ricardo Arrigoni”, vamos novamente dar um SELECT na tabela para poder ver o registro alterado

**Listagem 9**: SELECT para ver os dados atualizados

```
SELECT * FROM fornecedores;
```

![Editando registros](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL08.jpg)**Figura 5**: Editando registros.

Como vimos no exemplo anterior, estamos usando uma cláusula chama de WHERE em nosso SQL, essa cláusula é responsável por definir qual registro específico da tabela vai ser afetado pelo comando SQL.

### DELETE

Por último e não menos importante, vamos falar do comando DELETE. Ele é o responsável por remover todo e qualquer registro do bando de dados.

**Nota:**

Uma vez executado, esse comando não é reversível, portanto tome bastante cuidado ao deleter algum registro de seu banco de dados.

Agora que já sabemos o que ele faz e que devemos tomar muito cuidado ao utilizá-lo, vamos ver como usar ele em nosso exemplo.

**Listagem 10**: Deletando dados

```
DELETE FROM fornecedores WHERE codigo=3;
```

Saiba mais: [Comandos básicos em SQL - INSERT, UPDATE, DELETE e SELECT](https://www.devmedia.com.br/comandos-basicos-em-sql-insert-update-delete-e-select/37170)

Depois de executar esse comando o nosso registro de codigo=3 foi excluído do banco de dados e ele não poderá ser recuperado, ficamos então com apenas 2 registros em nossa tabela.

![Deletando dados da tabela](https://arquivo.devmedia.com.br/artigos/Ricardo_Arrigoni/MySQL/MySQL09.jpg)**Figura 6**: Deletando dados da tabela.

Como pudemos ver, o MySQL é um banco de dados bem simples e fácil de se usar, além de ser bastante leve e o melhor de tudo, gratuito. Por essas e outras que ele cresce cada vez mais tanto no mundo acadêmico quanto no mundo coorporativo.

Fico por aqui nesse tutorial, em breve mais tutoriais para os leitores do site da DevMedia, um abraço e até a próxima.

#### Confira também

[![Curso de MySQL](https://www.devmedia.com.br/arquivos/cursos/curso_criando-meu-primeiro-banco-de-dados-no-mysql_2200.png)Curso de MySQLCurso](https://www.devmedia.com.br/curso/curso-mysql/2200)

[![Introdução prática ao comando SQL SELECT](https://www.devmedia.com.br/arquivos/cursos/curso_introducao-pratica-ao-comando-sql-select_2199.png)Introdução prática ao comando SQL SELECTCurso](https://www.devmedia.com.br/curso/comando-sql-select/2199)

[![Avançando com Subqueries](https://www.devmedia.com.br/arquivos/cursos/curso_avancando-com-subqueries_2231.png)Avançando com SubqueriesCurso](https://www.devmedia.com.br/curso/curso-subqueries/2231)

AnotarMarcar como concluído