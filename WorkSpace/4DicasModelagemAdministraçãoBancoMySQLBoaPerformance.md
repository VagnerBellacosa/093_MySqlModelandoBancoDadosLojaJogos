# 4 dicas de modelagem e administração do banco MySQL para ter boa performance

Para garantir a boa performance de um banco MySQL é importante verificar alguns fatores. Veja aqui 4 dicas de modelagem e administração.



##### Autor: Redação Impacta

Data: 19/01/2016

------

Para efetuar a modelagem de um banco de dados é necessário entender bem o domínio da aplicação que utilizará o banco. Quando o assunto é a performance de um banco MySQL é importante verificar alguns fatores específicos como, por exemplo, a estrutura das tabelas, a sintaxe de consultas e a manipulação de cache. Confira a seguir 4 dicas que irão ajudar a melhorar a performance do seu banco de dados.

## **Administrando um banco MySQL via prompt**

Uma forma bem comum de administrar um banco de dados MySQL é através do prompt de comando no servidor onde o MySQL estiver instalado. Após executar o prompt, basta apenas digitar o comando “mysql -u root -p <senha do seu usuário root> ” e pronto. Será estabelecida uma conexão com o servidor MySQL, onde é possível, criar bancos, fazer consultas, alterações, inclusões e exclusões de dados.

## **Modelando um banco MySQL com o MySQL WorkBench**

Para criar um banco de dados é necessário antes fazer uma análise para identificar as tabelas e relacionamentos que serão necessários. Após possuir esse mapeamento, você já terá um diagrama do seu banco de dados. Esse diagrama é conhecido como diagrama entidade relacionamento (DER). Atualmente, existe uma ferramenta gráfica que poderá lhe ajudar a modelar o banco MySQL, o MySQL WorkBench, que, além de facilitar esse processo de modelagem de um banco, conta com a opção de exportar o código SQL necessário para criar o banco de dados com base no diagrama construído.

[![Algumas dicas podem te ajudar ao modelar um banco MySQL e garantir a boa performance](https://www.impacta.com.br/blog/wp-content/uploads/2016/01/shutterstock_233586214.jpg)](https://www.impacta.com.br/blog/wp-content/uploads/2016/01/shutterstock_233586214.jpg)

## **Administração de usuários**

É recomendado criar um usuário administrador para cada banco MySQL criado, utilizar o root em todos os bancos de dados não é recomendado. Além de aumentar a segurança do banco, ao se utilizar usuários diferentes, eles terão as permissões necessárias para administrar apenas aquele banco específico, enquanto o usuário root tem permissão elevada em todas as bases de dados do seu servidor MySQL. Também é muito importante definir privilégios específicos para os usuários do banco, por isso crie alguns perfis de usuário para servirem de base para a criação de novos usuários.

## **Otimização de consultas**

A otimização de consultas é uma excelente estratégia para melhorar a performance das consultas existentes no seu banco de dados. Uma das opções para fazer essa otimização é a criação de índices, onde uma coluna é definida para ser a identificadora dos dados da tabela. Após essa definição de um índice para uma tabela, a forma como os dados são pesquisados em uma tabela muda internamente, se tornando mais ágil. Outra opção muito indicada é analisar as consultas existentes para ver se elas retornam apenas os campos necessários. As consultas que retornam todos os campos de um registro demoram mais para serem executadas e, na maioria das vezes, alguns dados retornados não são utilizados.

Todas essas dicas anteriores podem ser muito úteis para melhorar a performance de um banco MySQL, mas lembre-se de que é importante fazer uma análise e um backup no seu banco de dados antes de fazer quaisquer alterações em sua estrutura. Tomando esses cuidados e utilizando essas dicas, você com certeza conseguirá otimizar a performance do seu banco de dados. Mesmo que, por exemplo, você diminua em um segundo a execução de determinada consulta, multiplique esse segundo pela quantidade de vezes que essa consulta será executada todo os dias durante um mês e você perceberá que o ganho foi muito grande!

## **Você deseja atualizar os seus conhecimentos ou virar um especialista em bancos MySQL?**

Então, confira os nossos cursos de[ MySQL – Módulo I](https://www.impacta.com.br/curso/MySQL-Modulo-I.php) e [MySQL – Módulo II](https://www.impacta.com.br/curso/MySQL-Modulo-II.php) e aprenda tudo para se tornar um administrador de bancos de dados de sucesso!