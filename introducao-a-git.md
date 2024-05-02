## Introdução - Criando histórias

- Adicionando um pedaço à história - Git status/add/commit/show
  git status                # ver o status atual
  git add .                 # adicionar todos os arquivos alterados
  git commit -m <titulo>    # criar um pacotinho com as modificações adicionadas
  git show                  # mostrar as informações do último commit


- Desfazendo pedaços da história - Git reset
  git reset HEAD~           # desfaz o último commit


- Lembrando da história - Git log
  git log                                     # lista os commits da branch atual
  git log --oneline                           # lista os commits apenas com o título
  git log -p                                  # lista os commits juntamente com as alterações
  git log -p <caminho-para-pasta-ou-arquivo>  # lista os commits que alteração o caminho especificado


- Explicando melhor as mudanças - Git commit com detalhes
  git commit            # cria um novo pacotinho de mudanças e abre um editor de texto para adicionar o título e detalhes
  git commit --amend    # adiciona alterações ao último pacotinho de mudanças


- Selecionando apenas alguns pedaços - Git add avançado
  git add -p                # seleciona "pedacinhos" das alterações um a um
  git add <file-or-folder>  # seleciona as alterações dos arquivos no caminho


- O que mudou? - Git diff
  git diff                            # diferença entre arquivos unstaged e index
  git diff --staged                   # diferença entre arquivos staged e HEAD
  git diff <ref1>                     # diferença entre o estado atual e um ref
  git diff <ref1> -- <file-or-folder> # diferença entre o estado atual e um ref para um caminho especifico
  git diff <ref1> <ref2>              # diferença entre duas refs
  git diff --name-only                # lista apenas o nome dos arquivos que mudaram


- Compartilhando histórias - Git push/pull
  git pull origin main  # puxa as atualizações do repositório remoto para o local
  git push origin main  # sobe as atualizações locais para o repositório remoto
