# gitHub
Branch criada com o intuito de estudo e documentação sobre o github

# Git github  

## GIT

Git: Global Infomation tracker

software de controle de versão

criado por Linus Torvalds - desenvolvedor do Kernel linux

Versionamento de codigo, software

Versões são muitas de uma mesma coisa, varios modos de como estão as coisas 

 commit: 
    quando se envia uma versão para um repositório local
    
 push: 
    quando se enviar o versionamento local para o remoto
    
 
 #### Vantagens:
  - controle de histórico
  - Trabalho em equipe
  - Ramificação do projeto
  - Segurança
  - Organização
 
 ## GitHub
  O git hub é um repositório local,
  a empresa criou uma rede social/comunidade
  
  Plataforma de rede sociais para programadores, onde os codigos ficarão salvos
    
  Baseado em Git

 - Repositórios ilimitados
 - Hospedagem de codigo-fonte
 - Características de rede social
 - GitHub Pages integrados
 - Colaboração
 - Forks

## Inicializando utilização
 Aqui trata-se sobre como é necessário configurar a maquina para a utilização do git e gitHub
 
 ### instalações
 
   git: https://git-scm.com/
 
 Aqui pode-se tomar duas diretivas, uma delas é utilizar uma interface gráfica, e a outra é utilizar um bash, ou terminal
  
   gitHubDesktop: https://desktop.github.com/
   
   Com essa feraamenta instala, ao inicializar, é preciso logar com a conta do gitHub
   
   Assim, pode-se já começar a manipular seu repositório remoto e local
   
   
   ### Usando o git 
   
   Aqui conterá a parte básica do uso do Git, porem dentro deste respositório, haverão demais arquivos contendo mais informações!
   
   #### criando um repositório
   Para começar a trabalhar com o git, é preciso cirar um repositprio para armazenar seus versionamentos realizados pelo GIT, para isso segue-se os passos:
   
   Se utilizando a interface gráfica, basta:
   
   - Na janela do programa, clica-se em cirar um novo repositório, e então precisa-se preencher os seguintes dados:
     - Name
     - Descrição
     - Local
     - git ignore
     - Licença 
    
  - Clica-se em `Criar repositório`
  - Para publicar esse repositório no repositório remoto, clica-se em `Publicar repositorio`
    - Assim, no seu GitHub já estará criado! 
   
  Se utilizando terminal, basta: 
  
  - Navegue, pelo terminal, até o diretório que se deseja salvar/manter os arquivos de versionamento do projeto
  - Execute o comando `git init`
  - Para enviar esse repositório para o remoto/GitHub, realize o processo de _pull_
 
 
   #### commit
   Durante a realização do seu trabalho, você realizará mudanças no seu codigo, através de um editor de texto de preferencia,
   essas mudanças ficaram salvas, porém não versionadas. Para poder versionar essas versões no seu **repositório local**,
   segue-se os seguintes passos
   
  Se utilizando a interface gráfica, basta
   - no canto inferior esquerdo, adicionar um nome e um comentario
   - clicar em `Commit to master` - esse _master_ irá mencionar qual branch você está
    
  
  Se utilizando o terminal, basta
   - Verificar se está no diretório do projeto
   - adicionar as mudanças -> `git add -p` ou `git add .`
   - commitar com o repositório local -> `git commit -m 'algum comentadio desejado'`
    
  #### push
  Assim se prossegue por várias situações, até em que chega o momento que você deseja alinhar/enviar as alterações feitas 
  por voce para o repositório remoto, para isso realize os seguintes passos:
   
   Se utilizando a interface gráfica, basta:
   - na pagina central da interface, irá aparecer um card sugerindo a descarga das anterações locais para o remoto
   - Neste card existirá um botão `Push origin`, então clica-se nele para realizar está ação
   - OBS: caso não haja push a ser feita, não aparecerá esta opção
    
   
   Se utilizando o terminal, basta:
   - Dentro do diretório do projeto, executa-se `git push`
    
  Pronto, agora seu remoto está alinhado com seu local.
  
  #### fetch
  Mas, e se houve alterações no remoto, ou outra pessoa adicionou/push de alterações no remoto, como faço pra atualizar no meu local?
  Para isso, é importante, sempre antes de começar alguema alteração, verificar se houve alterações e se há diferenenças entre o local e a origem/remoto
  A fim de se realizar essa operação, segue-se os passos:
   
   Se utilizando a interface gráfica, basta:
   - na parte superior da janela, possui-se um opção, como se fosse uma aba, com o titulo `Fetch origin`
   
   
   Se utilizando o termnial, basta:
   - no diretório do projeto, execute `git fetch`
   
   Observação impoetante: esse comando apenas identificará a diferenças da branch local com a remota, não irá realizar nenhuma alteração
   
  #### pull
  Havendo diferenças entre os repositórios local e remoto, é importante que baixe as atualizações feitas no remoto, para isso segue-se os passos: 
  
  Se utilizando a interface gráfica, bata:
  - Na pagina principal, aparecerá um cad sugerindo a opção de `Pull origin`, basta clica-lá
  - OBS: caso não haja pull a ser feita, não aparecerá esta opção

  Se utilizando o terminal, basta:
  - No diretório do projeto, execute `git pull`

  
  #### clone
  Haverá situações em que se mostra necessário que se pegue um projeto, um conjunto de arquivos no remoto, e você deseja trabalhar/executar eles em sua maquina, ou seja, localmente, permitindo então, que o seu git realize o versionamento de tal projeto (de forma local, na sua maquina), para isso, precisa-se executar os seguintes passos:
  
  - Navegue, por algum navegador, vá até o repositório em que deseja clonar
  - No canto direito, antes de mostrar os arquivos do mesmo, haverá um botão, normalmente em verde, com o titulo `Clone ou download`
  
  Se utilizando a interface gráfica, basta: 
  - Neste modal que apareceu nos passos anterioes, riá ter uma opção `abrir Desktop`
  - Clicando nele, já será aberto GitHubDesktop, porém contendo uma janela titulada como _Clone a repository_
  - Essa jenala mostrada, trará o repositório há ser clonado e o local, na sua maquina, seu será criada/salva os arquivos do projeto
  - Confirmado os dados, clique em `Clone`

  Se utilizando o terminal, basta: 
  - No terminal, navegue até o local em que deseja salrvar/baixar os arquivos do projeto
  - No modal mostrado no site, quando se clicou em `Clone or download`, terá um campo contendo uma URL (na aba HTTPS), copie essa URL
  - no terminal, digite `git clone <--a url_copiada_do_site-->`
  
 OBS: Quando se clona repositórios que não são seus, você pode tranquilamente realizar alterações locais, porém não será permitido que voce realise alterações no repositório de origem/remoto!
    
 # Definições importantes (e que te ajudará a compreender melhor)
 
   #### commit
    atualizar o repositório
   
   #### push
    dar uma descarga/decarregar, ou seja, empurrar aquele conjunto de alterações para o remoto
   
   #### pull
     trazer/puxar alterações
     
   #### fetch
     irá analisar a diferenças entre remoto e local, irá buscar atualizações do remoto
 
 # Curiosidades
  octodex: [octodex.github.com](https://octodex.github.com/)
 
 # Fonte de estudo
 https://www.youtube.com/playlist?list=PLHz_AreHm4dm7ZULPAmadvNhH6vk9oNZA
