# GitFlow TIFDRP

## Começando um repositório

GitHub:

- Criar o repositório

Máquina Local:

- Fazer um git clone na máquina:
  - `git clone git@repoaddress/repo.git`
- Criar um branch chamado develop:
  - `git checkout -b develop`
- Mandar o branch develop para o remoto:
  - `git push origin develop`
- Trackear o branch develop local o com develop remoto:
  - `git branch --set-upstream-to=origin/develop`

## Nova Funcionalidade

GitHub:

- Criar issue

Máquina local:

- Entrar no branch master e atualizá-lo:
  - `git checkout master`
  - `git pull`
- Entrar no develop e atualizá-lo:
  - `git checkout develop`
  - `git pull`
- Criar um branch novo para resolver a issue:
  - `git checkout -b issue-issueid`
- Commit das alterações:
  - `git add .`
  - `git commit -m "msg do commit resolve #issueid`
- Merge do branch da issue para develop:
  - `git checkout develop`
  - `git merge --no-ff issue-issueid`
- Mandar o branch develop pro remoto:
  - `git push origin develop`
- Ver se deu tudo certo no servidor de homologação:

GitHub:

- Entrar no branch develop
- Fazer Pull Request para master
- Se possível, pedir para alguém revisar o código
- Se estiver tudo ok com o código fazer um merge da PR para master
- Ver se deu tudo certo no servidor de produção
