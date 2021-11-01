## Português e Inglês / Portuguese and English

# Repository with Git commands
Markdown-style documentation repository with git commands

# Repositório com comandos Git
Documentação em Markdown com comandos git

<div align="left">
<img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="60" height="60"/>
</div>



## Link for Download / Link para Download
 <a href="https://git-scm.com/downloads"><img src="https://img.shields.io/badge/Git-330F63?style=for-the-badge&logo=git&logoColor=white" alt="Git"/></a>


### Comandos mais utilizados
Português

```

 git init
 git add .
 git commit -m "Primeiro Commit"
 git branch -M main
 git remote add origin <http://URL>
 git push -u origin main

 git checkout -b subMenu	
 git add.
 git commit -m "Alteracao Feita"
 git push -u origin subMenu

 git checkout main
 
 git diff subMenu..main

 git pull
 git merge subMenu
 git push
 
 
 git checkout subMenu
 git add .
 git commit -m "Testando Cherry Pick"
 git push -u origin subMenu
 git log
 
 
 git checkout main
 git cherry-pick f13bd3c3531f26e805c606729857f39987a2420f
 
 git branch -d subMenu
 git push origin --delete subMenu
 
 git reset [modo] [arquivo | commit]

```

### 
Most used commands

English

```

 git init
 git add .
 git commit -m "First Commit"
 git branch -M main
 git remote add origin <http://URL>
 git push -u origin main

 git checkout -b subMenu	
 git add.
 git commit -m "Change made"
 git push -u origin subMenu

 git checkout main
 
 git diff subMenu..main

 git pull
 git merge subMenu
 git push
 
 
 git checkout subMenu
 git add .
 git commit -m "Testing Cherry Pick"
 git push -u origin subMenu
 git log
 
 
 git checkout main
 git cherry-pick f13bd3c3531f26e805c606729857f39987a2420f
 
 git branch -d subMenu
 git push origin --delete subMenu
 
 git reset [mode] [file | commit]

```

## Português
### Breve explicação sobre cada um!

##### Criar um novo repositório
```
git init

```

##### obtenha um repositório
```
git clone <caminhoRepositorio>
```

##### Adicionar Um Arquivo Especifico
```
git add <arquivo>

```

#####  Adicionar Tudo que a de novo no repositorio local

```
git add .
git add *

```

##### Confirmar as Alterações

```
git commit -m "comentários das alterações"

```

##### Adicionar Um Caminho Remoto


```
git remote add origin git://suaUrl

```

##### Enviar Alterações para repositorio remoto

```

git push -u origin <NomeDaBranch>

```

##### Baixar Atualizações da branch remote pra local

```
git pull

```

##### Criar uma nova branch e a selecionar
```
git checkout -b <NomeDaBranch>

```
#### Adicionar Tudo Confirmando As Alterações e Enviando Para Repositorio 

```
git add.
git commit -m "Nova Alteração Da Branch"
git push -u origin <NomeDaBranch>

```

##### Voltando Para Branch Principal

```
git checkout <main>

```

##### mesclar alterações

```
git merge <NomeDaBranch>

```

##### Confirmar Merge

```
git push -u origin main

```

##### Baixar Atualição de branch Especifica 


```

git pull origin <NomeDaBranch>

```

##### Para pre visualizar alterações

```
git diff <BranchOrigem> <BranchDestino>

```

##### obter o id de commit 

```
git log

```

##### sobreescrever  alterações locais 


```
git checkout -- arquivo

```

##### remover todas as alterações e commits locais,
##### recupere o histórico mais recente do servidor e aponte para seu branch master local desta forma

```
 git fetch origin
 git reset --hard origin/main

```
##### excluir um repositorio

```
 rm -rf .git

```
##### remover uma pasta dentro do repositorio 

```
git rm -r NomeDaPasta

```

##### deletar uma branch local 

```
git branch -d <NomeDaBranch>

```


##### deletar uma branch remota 

```
git push origin --delete <NomeDaBranch>

```

#### Mostrar a diferenças entre arquivos


```
diff --git a/arquivo b/arquivo

```
##### Lista arquivos preparados, despreparados e que não foram monitorados.

```
git status

```

##### Remover Caminho Remoto E Adicionar Outra

```
git remote remove origin
git remote add origin git://suaUrl

```

##### Pegar Um Commit especifico para sua branch

```
git cherry-pick <IdDoCommit>

```

##### Pegar Commits Obtendo de um intervalo  

```
git cherry-pick <IdDoCommitInicial>^..<IdDoCommitFinal>

```

##### Resolver Conflitos cherry pick
##### Continue que é para você executar depois que resolver o conflito no código.
##### Abort, para cancelar o cherry pick.

```

git cherry-pick <IdDoCommit>

```

##### Desfazer alterações local ou remotamente 

```

git revert <NumeroHashOuId>

```

##### Alterar Caminho Remoto 

```
git cherry-pick --continue
git cherry-pick --abort

```
#### Desfazer mudanças no projeto após commits serem executados

```
git reset [modo] [arquivo | commit] 

```

## English
### Brief explanation of each one!

##### Create a new repository
```
git init

```

##### get a repository, clone repository
```
git clone <repositoryUrl>
```

##### Add a specific file
```
git add <file>

```

#####  Add everything new to the local repository

```
git add .
git add *

```

##### Confirm Changes

```
git commit -m "Change comments"

```

##### Add a remote path


```
git remote add origin git://YourUrl

```

##### Submit changes to remote repository

```

git push -u origin <NameBranch>

```

##### Download updates from remote branch to local

```
git pull

```

##### Create a new branch and select it
```
git checkout -b <NameBranch>

```
#### Add everything informing the changes and sending to repository 

```
git add.
git commit -m "New branch change"
git push -u origin <NameBranch>

```

##### Going back to main branch

```
git checkout <main>

```

##### Merge changes

```
git merge <NameBranch>

```

##### Confirm Merge

```
git push -u origin main

```

##### Download specific branch update 


```

git pull origin <NameBranch>

```

##### To preview changes

```
git diff <BranchOrigin> <BranchDestination>

```

#####  get commit id

```
git log

```

##### Overwrite local changes


```
git checkout -- file

```

##### Remove all local changes and commits,
##### Retrieve the latest server history and point to your local master branch like this

```
 git fetch origin
 git reset --hard origin/main

```
##### Delete a repository

```
 rm -rf .git

```
##### Remove a folder within the repository

```
git rm -r <folderName>

```

##### Delete a local branch

```
git branch -d <NameBranch>

```


##### Delete a remote branch

```
git push origin --delete <NameBranch>

```

#### Show the differences between files


```
diff --git a/file b/file

```
##### List prepared files, list of unprepared and unmonitored files.

```
git status

```

##### Remove remote path and add another

```
git remote remove origin
git remote add origin <git://YourUrl>

```

##### Get a specific commit for your branch

```
git cherry-pick <IdCommit>

```

##### Catch commits by getting from a range

```
git cherry-pick <IdCommitInitial>^..<IdCommitFinal>

```

##### Resolve cherry pick conflicts
##### Continue, which is for you to run after you resolve the conflict in the code.
##### Abort, to cancel the cherry pick.

```

git cherry-pick <IdCommit>

```

##### Undo changes locally or remotely

```

git revert <NumberHashOrId>

```

##### Change remote path

```
git cherry-pick --continue
git cherry-pick --abort

```

#### Undo project changes after commits are performed

```
git reset [mode] [file | commit]

```


#### Referencia link da documentação / References link documentation
<a href="https://git-scm.com/docs"><img src="https://img.shields.io/badge/Git-330F63?style=for-the-badge&logo=git&logoColor=white" alt="Git"/></a>
