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
