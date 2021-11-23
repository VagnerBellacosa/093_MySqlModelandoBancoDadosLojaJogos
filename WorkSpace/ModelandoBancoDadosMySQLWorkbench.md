# Modelando um banco de dados com o MySQL Workbench

[Favoritar](https://www.portalgsti.com.br/acoes-sociais/agir/xhr/4713/article/favourite?url_next=/2018/04/modelando-um-banco-de-dados-com-o-mysql-workbench.html)[Ver depois](https://www.portalgsti.com.br/acoes-sociais/agir/xhr/4713/article/see-later?url_next=/2018/04/modelando-um-banco-de-dados-com-o-mysql-workbench.html)[ Sugerir leitura](javascript:;)

[Facebook](http://www.facebook.com/sharer/sharer.php?u=https://www.portalgsti.com.br/2018/04/modelando-um-banco-de-dados-com-o-mysql-workbench.html&title=Modelando um banco de dados com o MySQL Workbench)[Twitter](http://twitter.com/intent/tweet?status=Modelando um banco de dados com o MySQL Workbench+https://www.portalgsti.com.br/2018/04/modelando-um-banco-de-dados-com-o-mysql-workbench.html)[Google+](https://plus.google.com/share?url=https://www.portalgsti.com.br/2018/04/modelando-um-banco-de-dados-com-o-mysql-workbench.html)[LinkedIn](http://www.linkedin.com/shareArticle?mini=true&url=https://www.portalgsti.com.br/2018/04/modelando-um-banco-de-dados-com-o-mysql-workbench.html&title=Modelando um banco de dados com o MySQL Workbench&source=portalgsti)

[![foto de ](https://img.portalgsti.com.br/F8jLXFH8Cb_f9uICjE9uryPvk5Q=/40x40/https://www.portalgsti.com.br/media/uploads/userprofile/2018/03/21/27973048_1576561145753927_2286952741924540363_n.jpg)](https://www.portalgsti.com.br/perfil/gabrielgoulart/)

[Gabriel Goulart](https://www.portalgsti.com.br/perfil/gabrielgoulart/)3 ANOS, 7 MESES ATRÁS

[4](javascript:void(0);)[0](javascript:void(0);)

[MYSQL](https://www.portalgsti.com.br/mysql/)



  O MySQL Workbench é uma ótima ferramenta para se criar banco de dados em SQL e muito fácil de usar. Com o Workbench instalado em seu computador clicamos em File -> New Model para começarmos a modelar nosso banco. Uma tela como essa irá aparecer:
![img](https://img.portalgsti.com.br/39PxbQSJvKK6DPJkTiJAosEUMt0=/708x0/https://www.portalgsti.com.br/media/uploads/gabrielgoulart/captura-de-tela-de-2018-04-19-08-42-58.png)

  Um duplo clique no cilindro amarelo escrito "mydb" nos permitirá mudar o nome do nosso banco. Coloque o nome que tiver mais coerência com o seu projeto e que te faça lembrar a que projeto aquele banco pertence. Feito isso vamos clicar em "Add Diagram". Em seguida teremos uma tela assim:
  ![img](https://img.portalgsti.com.br/MzSz7_d0xLfoNP8ojbZPmSSy2l4=/708x0/https://www.portalgsti.com.br/media/uploads/gabrielgoulart/captura-de-tela-de-2018-04-19-08-45-32.png)

  A partir daqui, se você tem conhecimento de banco de dados as coisas ficam bem fáceis. Nos últimos 6 itens temos as ferramentas de relação. Temos 1:1, 1:n e [n:m.](file:///N:/m.) A diferença entre a linha tracejada e a linha sólida é que a a primeira significa uma relação não identificável e a segunda uma relação identificável. Para criarmos uma tabela é só clicarmos no 7o item de cima para baixo e depois clicar no quadriculado. Uma tabela com o nome "table1" aparecerá. um duplo clique na tabela abrirá um retângulo com suas informações e abas. Para mudar o nome da sua tabela é só trocá-lo no campo Name. A aba columns é o nosso foco pois é nela que vamos popular nossa tabela com colunas e colocar os seus atributos.
  Depois de criar todas as suas tabelas com suas respectivas colunas e fazer as relações entre elas, para fazer a engenharia para frente e criarmos nosso sql é bem simples. Clicamos em file -> export -> Forward Engineer SQL Create Script, depois escolhemos onde vamos salvar nosso arquivo. Eu sempre marco as 2 primeiras caixas, mas fica a critério de cada um. Depois é só ir seguindo e teremos nosso SQL. Bem simples, não é mesmo?