# Versionando projetos antigos

Neste documento conterá uma explicação de como você tendo um projeto, feito sem o GIT, adicione-o no GIT

#### utilizando interface gráfica

Quando você utiliza a interface gráfica, as coisas ficam mais visuais, assim fica mais facil as ações.

Como primeiro passo, abra o aplicativo do GitHubDesktop,

Feito isso, verifique se você está na conta em que deseja realizar o upload do projeto - passo para quem possui mais de uma conta/organização no GitHub

Assim feito, nos menus da janela, que ficam na parte superior, existe um campo `File`, cliando nele, clica-se em `New repository...`

Assim ele abrirá uma nova janela sobreposta, que requisitará os seguintes dados
 - _Name_ - o nome
 - _Description_ - a descição
 - _Local Path_ - o diretório na sua maquina que será criada a pasta
 - _README_ - arquivo de descrição do repoistório
 - _Git Ignore_ - arquivos a serem ignorados de acordo com o que será inputado
 - _Lincense_ - a lincença a ser usada

Esses campos são necessários para cirar um novo repositório.

Para concluir a criação, clique em `Create repository`

**OBS**: esse repositório foi criado na sua maquina, ou seja, localmente, não havendo nenhuma conexão com o remoto!

Na janela gráfica, após os passos acima, aparecerá um card sugerindo a publicação do repositório local no remoto.

Assim ele mostrará uma janela para confirmar os dados antes de se realizar a publicação,

 - _Name_
 - _Description_
 - _Keep this code private_
 - _Organization_

Com isso verifique todos os dados e corrija-os caso necessário!

Confirmado os daods, clique em `Publish Repository`

Pronto, você já criou o repositório que receberá os arquivos, porém ele segue vazio, então agora iremos povoar esse repositório

Tendo esse repositório local, na sua maquina, basta que você cole os dados que deseja inputar nele, com sua devida organização desejada.

Automaticamente, quando você acessa novamente o Organizador GitHub, o GitHubDesktop, ele já identificará que há mudanças, locais, naquele repositório.

Tendo já, o git, identificado essas alterações, basta que realiza-se o **commit**, local, e para alinhar com o remoto, GitHub, realiza-se um **push**.

Dica: verificque se nãp há nenhum arquivo inútil que foi carregado junto. Caso haja, com o botão direito em cima do arquivo, selecionar a opção `Ignore File`.



#### utilizando terminal

... à completar

