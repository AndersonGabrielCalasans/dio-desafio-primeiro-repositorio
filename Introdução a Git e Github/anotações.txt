# Comandos usados no curso de Introdução a Git/GitHub:

 - git config

Um dos comandos git mais usados é o **git config** que pode ser usado para definir valores de configuração específicos do usuário como e-mail, algoritmo preferido para diff, nome de usuário e formato de arquivo etc. Por exemplo, o seguinte comando pode ser usado para definir o email:

_git config --global user.email sam@google.com_

 - git init

Este comando é usado para criar um novo repositório GIT. Uso:

_git init_

 - git add

O comando git add pode ser usado para adicionar arquivos ao índice. Por exemplo, o seguinte comando irá adicionar um arquivo chamado temp.txt presente no diretório local para o índice:

_git add temp.txt_

 - git clone

O comando git clone é usado para fins de verificação de repositório. Se o repositório estiver em um servidor remoto, use:

_git clone alex@93.188.160.58:/path/to/repository_

Por outro lado, se uma cópia de trabalho de um repositório local for criada, use:

_git clone /path/to/repository_

 - git commit

O comando git commit é usado para confirmar as alterações na cabeça. Tenha em atenção que quaisquer alterações efetuadas não irão para o repositório remoto. Uso:

_git commit –m “coloque sua mensagem aqui”_

 - git status

O comando git status exibe a lista de arquivos alterados juntamente com os arquivos que ainda não foram adicionados ou confirmados. Uso:

_git status_

git push é outro dos comandos git básicos mais usados. Um simples envio envia as alterações feitas para o ramo mestre do repositório remoto associado ao diretório de trabalho. Por exemplo:

_git push origin master_

 - git checkout

O comando git checkout pode ser usado para criar ramos ou alternar entre eles. Por exemplo, o seguinte cria um novo ramo e muda para ele:

_command git checkout -b <branch-name>_

Para simplesmente mudar de um ramo para outro, use:

_git checkout <branch-name>_

 - git remote

O comando git remote permite que um usuário se conecte a um repositório remoto. O comando a seguir lista os repositórios remotos atualmente configurados:

_git remote –v_

Esse comando permite que o usuário se conecte a um servidor remoto:

_git remote add origin <93.188.160.58>_

 - git branch

O comando git branch pode ser usado para listar, criar ou excluir ramos. Para listar todos os ramos presentes no repositório, use:

_git branch_

Para excluir um ramo:

_git branch –d <branch-name>_

 - git pull

Para mesclar todas as alterações presentes no repositório remoto para o diretório de trabalho local, o comando pull é usado. Uso:

_git pull_

 - git merge

O comando git merge é usado para mesclar uma ramificação no ramo ativo. Uso:

_git merge <branch-name>_

 - git diff

O comando git diff é usado para listar os conflitos. Para visualizar conflitos com o arquivo base, use

_git diff --base <file-name>_

O seguinte comando é usado para exibir os conflitos entre ramos about-to-be-merged antes de mesclá-los:

_git diff <source-branch> <target-branch>_

Para simplesmente listar todos os conflitos atuais, use:

_git diff_
_git tag_

A marcação é usada para marcar compromissos específicos com alças simples. Um exemplo pode ser:

_git tag 1.1.0 <insert-commitID-here>_

 - git log

Executar o comando git log exibe uma lista de compromissos em uma ramificação, juntamente com os detalhes pertinentes. Um exemplo de saída pode ser:

_commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw
Author: Alex Hunter <alexh@gmail.com>
Date:   Mon Oct 1 12:56:29 2016 -0600_

 - git reset

Para redefinir o índice e o diretório de trabalho para o estado do último commit, o comando git reset é usado. Uso:

_git reset --hard HEAD_

 - git rm

git rm pode ser usado para remover arquivos do índice e do diretório de trabalho. Uso:

_git rm filename.txt_

 - git stash

Provavelmente um dos menos conhecidos comandos git básicos é git stash que ajuda a salvar as mudanças que não devem ser cometidos imediatamente, mas em uma base temporária. Uso:

_git stash_

 - git show

Para visualizar informações sobre qualquer objeto git, use o comando git show. Por exemplo:

_git show_

 - git fetch

git fetch permite que um usuário obtenha todos os objetos do repositório remoto que atualmente não residem no diretório de trabalho local. Exemplo de uso:

_git fetch origin_

 - git ls-tree

Para exibir um objeto de árvore juntamente com o nome e o modo de cada item e o valor SHA-1 do blob, use o comando git ls-tree. Por exemplo:

_git ls-tree HEAD_

 - git cat-file

Usando o valor SHA-1, exiba o tipo de um objeto usando o comando git cat-file. Por exemplo:

_git cat-file –p d670460b4b4aece5915caf5c68d12f560a9fe3e4_

 - git grep

git grep permite que um usuário procure através das árvores de conteúdo frases e / ou palavras. Por exemplo, para pesquisar www.hostinger.com em todos os arquivos use:

_git grep "www.hostinger.com"_

 - gitk

gitk é a interface gráfica para um repositório local que pode ser invocado digitando e executando:

_gitk_

- git instaweb

Com o comando git instaweb, um servidor web pode ser executado em interface com o repositório local. Um navegador da Web também é automaticamente direcionado para ele. Por exemplo:

_git instaweb –httpd=webrick_

 - git gc

Para otimizar o repositório através da coleta de lixo, que irá limpar arquivos desnecessários e otimizá-los, use:

_git gc_

 - git archive

O comando git archive permite que um usuário crie um arquivo zip ou tar contendo os componentes de uma única árvore de repositório. Por exemplo:

_git archive --format=tar master_

 - git prune

Através do comando git prune, os objetos que não têm ponteiros de entrada são excluídos. Uso:

_git prune_

 - git fsck

Para executar uma verificação de integridade do sistema de arquivos git, use o comando git fsck. Todos os objetos corrompidos são identificados:

_git fsck_

 - git rebase

O comando git rebase é usado para reaplicação de compromissos em outro ramo. Por exemplo:

_git rebase master_