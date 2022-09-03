# Branches ou Ramificações

Esse é um tópico que julgo muito importante ter conhecimentos, pois isso pode te ajudar e/ou atrapalhar em seus projetos.

Para começar, é bacana pode entender desde o principio, então, traduzido do ingles, branch significa ramificação, e isso nos remete o pensamento em uma arvore, e essa é uma analogia muito boa.

Em uma arvore, temos o tronco principal, que na linguagem do git, normalente se nomea como _master_ ou _main_, ele é usado como seu produto principal, seu produto.

E deste ramo principal, pode-se, e vão, originar novas branchs, novas ramificações. Lembrando que esse branch _master_ é obrigatório no seu codigo.

As alterações realizadas nessas branches ramificadas, serão feitas somente nelas, nada será alterado nas demais branches, por isso que é mais seguro realizar esse processo.

Existe tambem o conceito de _origin_, que nada mais é o local onde você hospeda/guarda/backup do seu codigo, no nosso caso o GitHub.

Então, sabendo isso, podemos fazer alterações no nosso loca, _commits_ e, voce queira implementá-las no branch _master_, basta executar um _push_ e então estamos enviando essas alterações do _master_ local para o _origin_.

Como uma boa prática de uso do GIT, é que se evite _commits_ no ramo master, porque isso pode causar transtornos, por exemplo, voce está desenvolvendo uma nova funcionalidade do seu projeto e chega em um ponto que da um erro gigantesco e muito dificil, se voce estiver usando somente a _master_ você terá que fazer todo o processo de correção manual; mas se estiver utilizando uma ramificação da sua master, você pode, atraves do versionamento, voltar a uma versão mais estavél! 


Assim, toda vez que você for desenvolver, testar, corrigir, alterar ... crie um ramo/branch a partir do ramo principal. Finalizada esse desenvolvimento feito, essa Feature, e você deseja implementar essas alterações no ramo principal, realiza-se um __merge__, ou seja, irá mesclar uma branch com a outra.

![Imagem git branchs](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)

## Criando Branches

Temos algumas formas para se criar Branches, porém aqui darei o foco para as formas mais usadas

### Criando Branch GitHubDesktop

Abrindo então o aplicativo do gitHub, em sua tela principal, no topo, haverá uma linha com as informações de repositorio e branch que ele esta olhando. No card titulado como _Current branch_, ao clicar neste card, aparecerá uma janela sobreposta que as informações de todas as branches de tal repositório, a que você está e tambem a branch padrão. Ao canto direito desta tabela, existe um botão `Nre branch`, clica-se então.

Clicado em `Nre branch`, uma janela aparecerá ao centro da tela, requisitando o nome da nova branch (_Name_) e tambem uma questão muito importante, qual branch será usada como base para criar essa nova branch (_Create branch based on..._), ou seja, qual branch será seu ponto de partida para a nova. Selecionando uma opção e escolhando um nome. clique em `Create branch`.

Pronto, sua branch foi criada, mas não se esqeuça, que ela foi criada apenas no repositório local! Para empurrá-la para o remoto, basta publicar as alterações, que no caso do App GitHub, irá te sugerir assim que ela, a branch, for criada! 

### Criando Branch pelo terminal

Aqui o processo é mais facil um pouco, mas segue o mesmo fluxo da anterior.

No terminal bash, onde voce realiza os comandos git, dentro do seu diretório do projeto, você irá executar o seguinte comando:

    git checkout -b 'nome_nova_branch'
    
Pronto, aqui você já criou uma nova branch. Vale ressaltar que essa branch foi criada com base na branch que sua ferramenta de versionamento estava olhando.

## Trocando de branches

Temos algumas formas  para se locomover entre Branches, ou seja, trocar de branch, porém aqui darei o foco para as formas mais usadas

### Trocando a branch com GitHubDesktop

Na pagina do software GitHub, haerá, na parte superior, um card nomeado de _Current branch_, ele indicará em qual branch você está. Cliando nele, um modal será exibido mostrando todas as branches existentes naquele repositório e uma, marca com o check, indicando em qual ramificação está.

Para se alternar para outra branch, basta então, selecionar para qual Branch desejas ir.

Pronto, mudança de ramificação feita!

### Trocando a branch com terminal

Aqui o processo é mais facil um pouco, mas segue o mesmo fluxo da anterior.

No terminal bash, onde voce realiza os comandos git, dentro do seu diretório do projeto, você irá executar o seguinte comando:

    git checkout 'nome_branch_destino'
    
Pronto, mudança de ramificação feita!

## Mesclando branches

Aqui é quando se deseja realizar uma mescla entre dois branches, ou seja, quando se deseja levar informações de um branch para outro branch, esse processo é noemado, em ingles, como __merge__.

Como dito anteriormente, existem algumas formas de serem feitos, porém irei tratar somente das principais e mais usadas

### Mesclando branches utilizando GitHubDesktop

Tendo então as branches prontas para o merge, ou seja, todas as alterações já foram feitas e revisadas, vamos aos passos: 

 - No App GitHub, certifique-se que você está na branch que deseja receber as alterações, caso não esteja, realize um _chekcout_ (troca de branches).
 - No menu do topo, no item _Branch_, selecione a opção `merge into Current Branch`
 - Na janela aberta, será pedido para selecionar qual branch você deseja trazer para a branch que você está
 - Para realizar tal tarefa, clique no botão azul, no final da janela, `Merge <nome_Branch> into <nome_current_branch>`

OBS: esse merge foi realizado somente no seu repositório local, para alinhar/empurrar essas alterações, merge, com o origin, precisa-se realizar um __push__, que no caso do software, ele irá de sugerir tal ação.

### Mescalndo branches utilizando terminal

Aqui o processo é mais facil um pouco, mas segue fluxo parecido com o anterior.

No terminal bash, onde voce realiza os comandos git, dentro do seu diretório do projeto, verifique que a branch que você esteja será a que vai receber as alterações e então você irá executar o seguinte comando:

    git merge <nome_branch>
    
Pronto, merge feito!

### Conflitos

Em certas situações de mesclagens, quando existe mais de uma pessoa trabalhando em um codigo, ou ainda, que foi realizada uma alteração em uma mesma linha, poderá ocasionar um conflito, justamente porque uma linha foi mudada, alterando uma parte do código.

Nisto existem dois cenários:

 - Se estiver realizando o processo de merge via terminal
 - Se estiver realizando esse provesso via GitHubDesktop

Ambos reagiram da mesma forma, que é de te avisar e mostrar onde ocorreu o conflito, indicando que você resolva o mesmo antes de continuar com o processo de mesclagem.

#### No caso do __terminal__

Após a execução do comando, ele indicará, no nome do branch, que houve conflito, assim voce pode realizar essa correção no seu editor de texto preferido.

#### No caso do __GitHubDescktop__

Quando você seleciona um branch para puxar as alterações, ele já mostra um warning avisando que irá ocorre conflito. Caso queira continuar, pode-se clicar para realizar a ação do _merge_, trnaquilament, pois a partir daí, como no terminal, ele pedirá que você resolva os conflitos antes de continuar com o processo

COMENTÁRIO: recomendação de uso, para a correção dos conflitos, o VisualStudioCode, pois ele mostra visualmente as diferenças entre os códigos.

Finalizando as devidas correções, segue os passos para cada caso:

#### No caso do __terminal__

Será necessário: 
- Adidionar as alterações
- Realizar um commit 

#### No caso do __GitHubDescktop__

Será necessário apenas realizar um commit.

Lemrbando que essas alterações foram feitas somente no local, então é sugerivél que se realize um __push__

Pronto, tudo certo!

## Deletando Branch

Existe casos em que se faz necessário apagar uma branch, seja por um erro ou mesmo porque já não há mais neceddiade de mantê-la.

#### No caso do __GitHubDescktop__

- verifique se você está na Branch que deseja apagar
- No Tab Menu superior, em `Branch`, selecione `Delete...`
- No modal que será aberto, ele pedirá a confirmação da deleção, como forma de segurança
  - E ainda possui uma opção, `Yes, delete this branch on the remote`, Que se selecionada, deletará a branch do repositório remoto também.
- Para confrimar, pressione `Delete`

Pronto, branch deletada!

##### No caso do __terminal__

- Estando no diretório do projeto
- Verifique que você __não__ esteja na branch que deseja deletar
- Então execute o seguinte comando:

        git branch -d <nome_branch>
 
 OBS: o comando `-d` somente funcionara se seu _local_ está alinhado com o _remoto_
 
 - Para forçar a deleção mesmo sem o alinhamento de _local_ com _remoto_, execute

        git branch -D <nome_branch>
 
 OBS: esse comando realizou a deleção da branch somente no repositório local
 
 Caso queira realizar a exclusão do branch no repositório remoto, execute:
 
        git push <remoto> --delete <nome_branch>
 
 Branch remoto deletado! 
 
