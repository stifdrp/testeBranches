# GitFlow TIFDRP

## Começando um repositório

GitHub:

- Criar o repo

Máquina Local:

- Fazer um git clone na máquina:
  - `git clone git@repoaddress/repo.git`
- Criar um branch chamado develop:
  - `git checkout -b develop`
- Mandar esse branch para o remoto:
  - `git push origin develop`

## Contribuindo

GitHub:

- Criar issue

Na máquina local:

- Entrar na master e atualizar o branch local:
  - `git checkout master`
  - `git pull`
- Entrar em develop e atualizar o branch local
  - `git checkout develop`
  - `git pull`
- Criar uma branch nova para resolver a issue
  - `git checkout -b issue-issueid`
- Commit das alterações
  - `git add .`
  - `git commit -m "msg do commit resolve #issueid`
- Merge da branch da issue para develop
- Mandar develop pro Remoto
- Ver se deu tudo certo no servidor de homologação

GitHub:

- Fazer Pull Request para master
- Ver se deu tudo certo no servidor de produção