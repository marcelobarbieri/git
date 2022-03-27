# Git

<details><summary>Fundamentos de DevOps</summary>

## Controle de Versão

### 1. Controle de Versão Local

#### 1.1 Setup

    git init
    dotnet new gitignore

#### 1.2 Versionando o projeto

    git add --all
    git status
    git commit
    git log

<br>

### 2. Controle de versão remoto

#### 2.1 Enviando o repositório local para um remoto

    git remote https://
    git push

#### 2.2 Copiando um repositório remoto

    git clone

<br>

### 3. Trabalhando com equipes

#### 3.1 Sincronizando um repositório remoto com o local

    git pull

#### 3.2. Ramificando o projeto

    git branch
    git checkout

</details>

<details><summary>Quick Setup</summary>

Create a new repository on the command line:

    echo "# teste" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/marcelobarbieri/teste.git
    git push -u origin main

</details>

<details><summary>Remove Commit</summary>

### 1. The last commit

Reset the HEAD

    git reset --hard HEAD^

#### Git remove the last commit by resetting the HEAD

It is simple to remove the last commit in history.
You can reset HEAD by running the command.

The caret **^** after HEAD implies the last commit referencing the **HEAD**.

### 2. A group of commits on a branch

Interactively rebase the branch

    git rebase -i HEAD~N

where **N** is the number of commits from the head

or

git squash the commits

    git merge --squash <branch>

### 3. All commits

Navigate to the folder hosting the repo and delete **.git** subdirectory

    rm -rf .git

### 4. Remove the only (one) commit you have.

    git update-ref -d HEAD

The challenging part about understanding git remove commits lies in having inadequate knowledge of git workflow, the reset command and branching. Here is what you should know about the three things.

[GoLinuxCloud](https://www.golinuxcloud.com/git-remove-commit/#:~:text=Reset%20is%20the%20most%20familiar%20command%20to%20git,deletes%20the%20associated%20files%20in%20the%20working%20directory.)

</details>
