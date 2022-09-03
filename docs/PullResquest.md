# Pull Resquest

Neste documento, trarei informações sobre Pull Requests do GitHub, o que são, porque utilizá-los, como utilizá-los e demais informações.

### O que é Pull Resquest?

Pull request, no seu sentito literal é _solicitar uma puxada_, mas o que isso quer dizer, para o GitHub, uma pull request, como seu proprio nome diz, é quando se realiza uma requisição, um pedido, para realizar um pull de certas mudanças. 

Tá, isso ficou complexo, então vamos para um exemplo:

Suponhamos que você trabalha em uma empresa, e nela possui um projeto que varias pessoas modificam. 
Esse projeto possui uma versão, branch, que representa a versão de homologação, ou seja, um versão, que serve para testar atividades. features, realizadas.
Porém, precisa-se que um mediador, analise as alterações feitas antes de permitir a entrada delas no branch de testes.
Assim a Pull resquest entra nesse ponto, quando se finaliza alterações realizadas em uma ramificação (trataremos disso em outro documento), e precisa pedir uma revisão para alguém afim de que essas alterações sejam validadas e adicionadas ao branch em questão.

Sendo assim, de forma resumida, podemos dizer que é uma forma de dizer a alguem que voce finalizou uma alteração.

Uma Pull Request (chamada tambem de PR) realiza um merge, mesclagem, entre duas Branchs, ou seja, irá implementar as mudanças feitas em uma branch em outra. Porem essa mudança só é permitida quando a PR for aceita pelo revisor. existe situações que não precisa-se da aprovação de um revisor, porem isso não é uma boa prática!

Depois que uma Pull request foi aberto, pode-se realizar correções de conflitos gerados, comentários e discussões.

Na pagina da PR, também é possivel analisar todas as mudanças que a branch ferá na branch de destino, que será feita a mesclagem! 

### Criando uma Pull Request

Pode-se criar uma PullRequest de algumas formas, trarei algumas, mais conhecidas.

#### Web browser - Navegador

Caso você opte por essa opção, de usar um navegador, é preciso que esteja logado em uma conta e que esta tenha permissão de gravação nos branchs envolvidos no pull request.

Na pagina do repositório, existirá um menu na parte superior aos arquivos, um menu de abas. Neste menu, é preciso clicar na opção `Pull requests`. Clicando no botão, você será redirecionado à uma segunda página que conterá todos os pull requests, sendo padrão um filtro de PR abertas, mas esse pode ser modificado para filtrar da forma como deseja!

Para realizar um novo PR, ao canto direito, possui então o botão, em verde, de `New pull request`, clicando nele aparecerá uma nova janela que pedirá para você dizer qual Branch você quer mesclar com qual. Ao selecilar os branchs desejados, eles precisam ser diferentes, irá aparecer todas as alterações que seram feitas. De acordo com isso, basta então que clicar em `Create pull request`, que estará em verde no canto direito. Feito isso, novamente voce será redirecionado para um outra pagina em que tera opções de complementos de informações, como um titulo e um comentário (Sugiro que completem bem esses campos, pois eles podem te ajudar no futuro), e tambem haverá configuraçõs na coluna a direita, como por exemplo adicionar uma pessoa para revisar e aprovar, tags, label entre outras. Preenchido os campos, so clicar em `Create pull request` no cato inferior direito da caixa de texto.

Dependendo de como foi configurada as branchs, poderam acontecer de varias formas os proximos passos, poderá permitir que voce mesmo aceite o PR ou que necessite da revisão de outra(s) pessoa(s) para tal.

Caso haja conflitos, sugiro que você mesmo os corrijam, uma vez que foi voce quem realizou tais alterações, então está mais ciente das partes mais importantes do codigo.

Com tudo certo, basta realizar o merge, clicando em `Merge pull request`, que estará em verde, caso revisado por outro, ao final do relatório de ações feitas.

#### Desktop GitHub

Neste caso, as coisas são bem simples, pois na pagina central do aplicativo, quando houver alterações entre branchs e possiveis de serem feitas, irá existir um card sugerindo que voce faça um pull request. Caso deseja, clicando no botão azul no canto direito do card, `Create Pull Request`, voce será redirecionado para a tela do navegador. A partir daqui, repete-se os mesmos passos citados no item anterior. 

#### GitHUb CLI - terminal

Aqui as coisas ficaram menos visuais, pois todos os passos serão atraves de comandos.

Estando no diretório do projeto, considerando que o git e gitHub já estão configurados corretamente, segue-se os passos:

 - para criar um pull request: `gh pr create`
 - para adicionar um revisor ao PR: `gh pr create --reviewer monalisa,hubot  --reviewer myorg/team-name`
 - Para indicar os branchs: `gh pr create --base my-base-branch --head my-changed-branch`
 - Para adicionar um titulo: `gh pr create --title "The bug is fixed" --body "Everything works again"`
 - Para cirar um PR no navegador: `gh pr create --web`

