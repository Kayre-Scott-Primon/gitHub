# Branches ou Ramificações

Esse é um tópico que julgo muito importante ter conhecimentos, pois isso pode te ajudar e/ou atrapalhar em seus projetos.

Para começar, é bacana pode entender desde o principio, então, traduzido do ingles, branch significa ramificação, e isso nos remete o pensamento em uma arvore, e essa é uma analogia muito boa.

Em uma arvore, temos o tronco principal, que na linguagem do git, normalente se nomea como _master_ ou _main_, ele é usado como seu produto principal, seu produto.

E deste ramo principal, pode-se, e vão, originar novas branchs, novas ramificações. Lembrando que esse branch _master_ é obrigatório no seu codigo.

Existe tambem o conceito de _origin_, que nada mais é o local onde você hospeda/guarda/backup do seu codigo, no nosso caso o GitHub.

Então, sabendo isso, podemos fazer alterações no nosso loca, _commits_ e, quando executamos um _push_ estamos enviando essas alterações do _master_ local para o _origin_.

Como uma boa prática de uso do GIT, é que se evite _commits_ no ramo master, porque isso pode causar transtornos, por exemplo, voce está desenvolvendo uma nova funcionalidade do seu projeto e chega em um ponto que da um erro gigantesco e muito dificil, se voce estiver usando somente a _master_ você terá que fazer todo o processo de correção manual; mas se estiver utilizando uma ramificação da sua master, você pode, atraves do versionamento, voltar a uma versão mais estavél! 


Assim, toda vez que você for desenvolver, testar, corrigir, alterar ... crie um ramo/branch a partir do ramo principal. Finalizada esse desenvolvimento feito, essa Feature, e você deseja implementar essas alterações no ramo principal, realiza-se um __merge__, ou seja, irá mesclar uma branch com a outra.

![Imagem git branchs](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)

