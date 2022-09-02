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
   
   ### Criando um novo repositorio
   
   Na janela do programa, clica-se em cirar um novo repositório, e então precisa-se preencher os seguintes dados:
   
   - Name
   - Descrição
   - Local
   - git ignore
   - Licença 
    
   Clica-se em `Criar repositório`
 
   Para publicar esse repositório no repositório remoto, clica-se em `Publicar repositorio`
   
   Assim, no seu GitHub já estará criado! 
   
   
   ### Usando o git 
   
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
    
  Assim se prossegue por várias situações, até em que chega o momento que você deseja alinhar/enviar as alterações feitas 
  por voce para o repositório remoto, para isso realize os seguintes passos:
  
   
   Se utilizando a interface gráfica, basta:
   - na pagina central da interface, irá aparecer um card sugerindo a descarga das anterações locais para o remoto
   - Neste card existirá um botão `Push origin`, então clica-se nele para realizar está ação
   - OBS: caso não haja push a ser feita, não aparecerá esta opção
    
   
   Se utilizando o terminal, basta:
   - Dentro do diretório do projeto, executa-se `git push`
    
  Pronto, agora seu remoto está alinhado com seu local.
  
  Mas, e se houve alterações no remoto, ou outra pessoa adicionou/push de alterações no remoto, como faço pra atualizar no meu local?
  Para isso, é importante, sempre antes de começar alguema alteração, verificar se houve alterações e se há diferenenças entre o local e a origem/remoto
  A fim de se realizar essa operação, segue-se os passos:
  
   
   Se utilizando a interface gráfica, basta:
   - na parte superior da janela, possui-se um opção, como se fosse uma aba, com o titulo `Fetch origin`
   
   
   Se utilizando o termnial, basta:
   - no diretório do projeto, execute `git fetch`
   
   Observação impoetante: esse comando apenas identificará a diferenças da branch local com a remota, não irá realizar nenhuma alteração
   
  Havendo diferenças entre os repositórios local e remoto, é importante que baixe as atualizações feitas no remoto, para isso segue-se os passos: 
  
  Se utilizando a interface gráfica, bata:
  - Na pagina principal, aparecerá um cad sugerindo a opção de `Pull origin`, basta clica-lá
  - OBS: caso não haja pull a ser feita, não aparecerá esta opção

  Se utilizando o terminal, basta:
  - No diretório do projeto, execute `git pull`

  
   
  
    
 # Definições importantes (e que te ajudará a compreender melhor)
 
   #### commit
    atualizar o repositório
   
   #### push
    dar uma descarga/decarregar, ou seja, empurrar aquele conjunto de alterações para o remoto
   
   #### pull
     trazer/puxar alterações
 
 # Curiosidades
  octodex: [octodex.github.com](https://octodex.github.com/)
 
 # Fonte de estudo
 https://www.youtube.com/playlist?list=PLHz_AreHm4dm7ZULPAmadvNhH6vk9oNZA
