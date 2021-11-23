# Modelagem de dados WorkBench MySQL

100 visualizaçõesCOMPARTILHE!

### [CAMILO LOPES](https://imasters.com.br/perfil/camilo_lopes)

Tem [175 artigos](https://imasters.com.br/back-end/modelagem-de-dados-workbench-mysql#) publicados com[ 3111576 visualizações](https://imasters.com.br/back-end/modelagem-de-dados-workbench-mysql#) desde [2011](https://imasters.com.br/back-end/modelagem-de-dados-workbench-mysql#)

[![Camilo Lopes](https://secure.gravatar.com/avatar/3ce8d8a11a1fde040a921671a252fb3f?s=96&d=mm&r=g)](https://imasters.com.br/perfil/camilo_lopes)

### [CAMILO LOPES](https://imasters.com.br/perfil/camilo_lopes)

175

é Bacharel em Sistemas de Informação e Especialista em Gestão e Estratégia de Negócios. Trabalha com TI desde 2003 e possui as certificações SCJP 5 e SCM. Trabalhou na IBM Brasil como Analista Programador Java, passou pelo laboratório da Enterprise Computing Lab (ECL) HP como Software Engineer, Ci&amp;T como Engenheiro de Software em projeto JEE. Tem experiência internacional em Índia, Dubai e Londres. Atualmente é cofundador da ITSLabs (www.itslabs.com.br), uma start-up focada na criação de produtos web e mobile para start-ups. Também é autor dos livros "Guia do Exame SCJP", "Guia Prático JEE com Frameworks" e "TDD na prática".

[LEIA MAIS](https://imasters.com.br/perfil/camilo_lopes)

18 MAR, 2015

### [Série AngularJS: Atualizando versão do AngularJS via Yeoman](https://imasters.com.br/front-end/serie-angularjs-atualizando-versao-do-angularjs-via-yeoman)

11 MAR, 2015

### [Usando Yoeman com AngularJS](https://imasters.com.br/front-end/usando-yoeman-com-angularjs)

4 MAR, 2015

### [Série AngularJS: criando blackList com Angular-ui validate](https://imasters.com.br/front-end/serie-angularjs-criando-blacklist-com-angular-ui-validate)

Olá, pessoal.

No artigo de hoje, vou falar sobre uma ferramenta para modelagem de dados que substituiu o DBDesigner 4. É o WorkBench (WB). Através deste conteúdo vamos conhecer um pouco a ferramenta e também vou mostrar de modo pratico algumas funcionalidades.

Não posso deixar de mencionar que há outras ferramentas pagas excelentes e a vantagem da aquisição destas é quando você precisa usar algo que não seja tão trivial e o WB não atende. Mesmo assim, vale conferir os benefícios do WorkBench. Me acompanhe em cada etapa!

#### Starting…

O WorkBench é uma ferramenta da Sun criada para fazer a modelagem de dados em banco de dados MySQL. A ferramenta substitui uma das mais famosas ferramentas free em modelagem de dados, o DBDesingner4.

O projeto DBDesingner4 foi descontinuado e o WorkBench assumiu a liderança. Abaixo listamos algumas vantagens da ferramenta:

- Gratuita para uso sem restrições;
- Disponível para Windows, Linux e OS X;
- Ótima documentação, bem organizada e com uma linguagem simples para os iniciantes;
- Pouco consumo de memória;
- Permite fazer engenharia reversa;
- Conexão direta com o banco de dados;
- Exportar em vários formatos do mercado: PNG, PDF e SVG.
- Baixa curva de aprendizado.

No site do [WorkBench](http://wb.mysql.com/) você pode fazer o download da versão mais recente, ter acesso aos tutoriais, documentação etc.

#### Fazendo Engenharia Reversa MySQL & WorkBench

Veremos neste tópico como comunicar WorkBench com um Base de Dados no MySQL. Só assim poderemos importar tabelas e sincronizar as informações, como também podemos fazer as alterações no WorkBench e refletir no nosso Banco de Dados.

Então, vamos primeiramente importar as tabelas que criamos (empregado e cargo) no capítulo de Banco de dados. Para isso, faremos a engenharia reversa. Veja na imagem a seguir:
![img](http://conteudo.imasters.com.br/20668/36160.jpg)
Na próxima tela, precisamos informar ao WorkBench os dados da conexão, então informe a conexão local, o username e o password. Em seguida, clique em next duas vezes.

Na terceira tela, precisamos escolher quais schema e também vamos importar a(s) tabela(s). Selecione o schema em que se encontram as tabelas que criamos ainda há pouco. Clique em next e vá para ultima tela. A partir daí, vamos poder escolher quais tabelas vamos importar do schema. Confira:
![img](http://conteudo.imasters.com.br/20668/36161.jpg)
Escolhemos apenas as tabelas que nos interessam. Em seguida, clique em execute. Depois clique em next duas vezes para finalizar. Ao fazer isso, você tem a imagem a seguir, que representa as tabelas e que nesse caso há um relacionamento entre elas:
![img](http://conteudo.imasters.com.br/20668/36162.jpg)
Para editar qualquer uma das tabelas, basta dar dois cliques sobre elas. Pronto! Assim criamos nossa modelagem diretamente do banco de dados usando a engenharia reversa. Podemos exportar nossa modelagem para PDF, JPG, GIF – mais uma vantagem da ferramenta.

Vou ficando por aqui, e no próximo artigo, vou mostrar como sincronizar dados do WorkBench com o MySQL.

Espero que tenha gostado do conteúdo com cada etapa da modelagem de dados WorkBench. Compartilhe suas impressões e os testes nos comentários para termos um feedback desta ferramenta.

Abraços e até a próxima!

![img](https://imasters.com.br/assets/images/commons/owl.png)