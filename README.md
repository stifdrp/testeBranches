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

Máquina local:

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
  - `git checkout develop`
  - `git merge --no-ff issue-issueid`
- Mandar develop pro Remoto
  - `git push origin develop`
- Ver se deu tudo certo no servidor de homologação

GitHub:

- Entrar no branch develop
- Fazer Pull Request para master
- Se possível, pedir para alguém revisar o código
- Se estiver tudo ok com o código fazer um merge da PR para master
- Ver se deu tudo certo no servidor de produção
