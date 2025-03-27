# DIO | Git e Github

Repositório para armazenar informações sobre Git e Github - Curso da DIO [Digital Innovation One] (https://www.dio.me)

## Documentação

- [Documentação Git] (https://git-scm.com/docs)
- [Documentação Github] (https://docs.github.com)

## Comandos git

Criando um repositório local:
1.1 Criar o diretório
1.2 usar o comando "git init"

"git status"-> exibe o status atual do repositório.
"git remote -v" -> exibe o repositório remoto associado ao diretório aual (se houver).
"git remote add origin <URL> -> associa o diretório local ao repositório remoto apontado no comando.
"cat config" -> no diretório .git, exibe as informações do git para o diretório em uso.
"git clone <URL> <nome diretório local> -> clona um repositório do Github para o diretório em uso (nomeando o diretório com o nome do repo remoto ou com o nome do diretório informado no comando).
"git clone <URL> --branch <nome da branch no repo remoto> --single-branch -> clona um repositório do Github para o diretório em uso (apenas a branch informada)
"git log" -> exibe informações sobre os commits do repositório.

Para remover o git criado indevidamente, remover o diretório '.git' -> no linux: rm -rf .git

"git commit --amend -m <nova msg> -> altera a msg do último commit

"git reset --soft <hash desejado>" -> retorna o ponteiro do git para o commit informado no <hash>, retornando os arquivos posteriores ao <hash> para a área de preparação (staging area).

"git reset" ou "git reset --mixed <hash>" (comportamento padrão do git reset) -> retorna o ponteiro do git para o commit informado no <hash>, retornando os arquivos posteriores ao <hash> para a área de trabalho (working area).

"git reset" ou "git reset --hard <hash>" (comportamento mais radical do git reset) -> retorna o ponteiro do git para o commit informado no <hash>, mas apaga os arquivos posteriores ao <hash>.

"git reset <nome do arquivo>" -> retorna o arquivo informado para a área de trabalho.

"git restore <nome do arquivo>" -> faz o mesmo que o git reset.

"git reflog" -> exibe as informações de todas as interações realizadas nos commits.

"git checkout -b <nome da nova branch> -> cria novo branch.

"git checkout <nome da branch> -> vai para a branch informada no comando.

"git branch -v" -> mostra todas as branchs para o repositório em que se está trabalhando.

"git merge <nome da branch>" -> mescla a branch informada com a branch principal do repositório.

"git branch -d <nome da branch>" -> exclui a branch informada no comando.

"git fetch origin <nome da branch>' -> baixa as alterações do repositório remoto, sem fazer o merge com o repositório local.

"git diff <nome da branch1> <nome da branch2>" -> exibe as diferenças entre o conteúdo das branchs apontadas no comando. Para atualizar, usar o comando "git merge <nome da branch>".

"git stash" -> 'arquiva' a modificação realizada na branch (permitindo criar nova branch, por exemplo).

"git stash list" -> 'lista' as modificações arquivadas.

"git stash pop" -> traz a modificação arquivada, removendo-a da 'pilha'.

"git stash apply" -> traz a modificação arquivada, mantendo-a na 'pilha' para eventual uso posterior.

"git pull" -> baixa informações do repositório remoto para o repositório local.

"git pull upstream <branch>" -> baixa informações do repositório configurado como upstream (exemplo: quando se faz um fork mas se deseja
alterações do repositório original).

"git push" -> envia informações do repositório local para o repositório remoto.
