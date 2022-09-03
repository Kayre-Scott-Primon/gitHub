# Comandos mais usados

Aqui é uma área onde eu irei colocar alguns comandos mais usados. Ela se destina a quem usa o git e GitHub via terminal, seja no Linux, Windows ou até memso Mac!

## Versão

Para mostrar a verão do codigo

    git --version

## Configuração

Para configurar um repositório _remoto_ no _local_

    git remote add origin <url_project_gitHub>

Ou seja, está adicionando o _remoto_ no _origin_

## Inicializando repositótio local

Para se criar um repositório local, esse comando deve ser executado dentro da pasta em que deseja criar o mesmo

    git init
    
ou ainda, estipulando um nome

    git init <nome do repositório>

Essa ação cirará tambem uma branch, a branch padrão.

## Status

Para mostrar o estado de cada arquivo dentro do repositório

    git status
    
## Add

Para se adicionar um arquivo para ser versionado

    git add <nome_arquivo>
    
ou, para adicionar todos de uma vez

    git add .

ou, para verificar as mudanças antes de adicionar

    git add -p
    
## Commit

Para realizar commit, ou seja, para adicionar uma alteração feita no repositorio local

    git commit
    
ou, para ja adicionar um comentário

    git commit -m "comentádio"

## log

Para ver todos os commits do branch

    git log

## Show

Quando se deseja informações mais detalhas sobre os commits

    git show <ID_commit>

## diff

Quando se deseja visualizar as diferenças de um arquivo neste repositório, mudanças essas que ainda não foram commitadas

    git diff <nome_arquivo>
    
## Push

Para enviar as alterações feitas no _local_ para o _remoto_

    git push
    
ou ainda, passando o _local_ e o _remoto_, respectivamente

    git push origin master

ou ainda quando não existe a branch no _remoto_

    git push --set-upstream <nome> <nome_branch>

## Pull

Para trazer alterações feitas no _remoto_ para o _local_

    git pull
    
ou ainda, passando o _local_ e o _remoto_, respectivamente

    git pull origin master

## Clone

Para baixar um projeto do _remoto_ para o _local_

    git clone <url_projeto_gitHub>
    
## Branch

Para visualizar as branches do repositório

    git branch
    
## Cirar branch

Para criar uma branch, a partir da que você está

    git branch <nome_da_branch>
    
## Deletar branch

Para deletar uma branch, desde que não seja a que você está

    git branch -d <nome_da_branch>

## Mudar de branch

Para alternar para outra branch

    git checkout <nome_da_branch>
    
## Cirar Branch

Para se criar uma branch, a partir da que está, e alternando para a nova

    git checkout -b <nome_nova_branch>
    
## Conexão com _remoto_

Para se estabelecer uma conexão com o repositório remoto

    git remoto add <nome> <url_repositorio>
    
## Fetch

Quando se deseja que o repositório local olhe para o remoto

    git fetch
    
## Stash

Quando se deseja armazenar temporariamente algum arquivo modificado, como se fosse esconde-lo por algum momento

    git stash
    
### List

Para listar os arquivos escondidos

    git stash list
    
### Pop

Para trazer os arquivos escondidos

    git stash pop
    
ou ainda

    git stash apply
    
## Rm

Quando se deseja remover arquivos da pasta so repositório

    git rm <nome_arquivo>
    
## Help

Quando se está em duvida sobre as ações de um comando

    git help <comando>

## Merge

Quando se deseja mesclar uma branch com a que você está

    git merge <nome_branch>

## Revert

Para desfazer commits

    git revert '<ID_commit>'

## Reset

Outra forma de desfazer ações/commits, ou retornar para um certo ponto

- Voltar para o ultimo commit

      git reset --hard HEAD~1
      
- Voltar para o ultimo commit mas manter os arquivos como não versionados

      git reset --soft HEAD~1
      
- Voltar para um commit especifico

      git reset --hard <ID_commit>
      
# Todos os comandos do Git

[Git comandos](https://git-scm.com/docs/git/pt_BR)

## Fontes

- [Video rocketseat - Principais comandos Git](https://www.youtube.com/watch?v=E28J23gCBIs)
- [CodigoFonte](https://www.codigofonte.com.br/artigos/top-25-comandos-do-git)
- [Geekhunter](https://blog.geekhunter.com.br/comandos-git-mais-utilizados/)
- [Comandos Git - Git](https://comandosgit.github.io/)
