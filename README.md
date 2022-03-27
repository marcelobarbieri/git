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
