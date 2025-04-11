# Atividade Avaliativa - Git Colaborativo com Portugol

## Integrantes do grupo
- João Victor Martins Ferro
- Fernando Ancioto
- Pietro Filla

## Objetivo
Desenvolver colaborativamente um algoritmo em Portugol de soma e subtração

## Etapas realizadas por cada membro

### João Victor
- Como criou?
  Primeiro criei um repositório no GitHub, com o nome de "AtividadeFinal"; depois adicionei o Fernando e o Pietro como colaboradores; e por fim adicionei o "algotitmo.por"
  
- Como Configurou o Git? não deixe exposto sua chave.
  
compuni@Lab6m13 MINGW64 ~
$ git config --global user.name Joao

compuni@Lab6m13 MINGW64 ~
$ git config --global user.email joaovictor.mafer@gmail.com

compuni@Lab6m13 MINGW64 ~
$ ssh-keygen -t rsa -b 4096 -C joaovictor.mafer@gmail.com
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/compuni/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/compuni/.ssh/id_rsa
Your public key has been saved in /c/Users/compuni/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:669tXatjc1ZO8BYiP5/MLWF7ve+n01j3IBGtQgY2NXg joaovictor.mafer@gmail.com
The key's randomart image is:
+---[RSA 4096]----+
|        ++o  .   |
|       ...E.. .  |
|         +   o   |
|          ..o... |
|        S  .o..o.|
|         .  .o= B|
|        .  . +=&*|
|       . .. = O=O|
|        o+o..*.B*|
+----[SHA256]-----+

compuni@Lab6m13 MINGW64 ~
$ eval "$(ssh-agent -s)"
Agent pid 954

compuni@Lab6m13 MINGW64 ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/compuni/.ssh/id_rsa (joaovictor.mafer@gmail.com)

compuni@Lab6m13 MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

compuni@Lab6m13 MINGW64 ~
$ ssh -T git@github.com
Hi JoaoFerro17! You've successfully authenticated, but GitHub does not provide shell access.

compuni@Lab6m13 MINGW64 ~
$ git clone git@github.com:JoaoFerro17/AtividadeFinal.git
Cloning into 'AtividadeFinal'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.

compuni@Lab6m13 MINGW64 ~
$ cd AtividadeFinal

compuni@Lab6m13 MINGW64 ~/AtividadeFinal (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   algoritmo.por

no changes added to commit (use "git add" and/or "git commit -a")

compuni@Lab6m13 MINGW64 ~/AtividadeFinal (main)
$ git add .

compuni@Lab6m13 MINGW64 ~/AtividadeFinal (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   algoritmo.por


compuni@Lab6m13 MINGW64 ~/AtividadeFinal (main)
$ git commit -m "Primeira modificação - por João"
[main aa74a2b] Primeira modificação - por João
 1 file changed, 1 insertion(+), 1 deletion(-)

compuni@Lab6m13 MINGW64 ~/AtividadeFinal (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 355 bytes | 355.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:JoaoFerro17/AtividadeFinal.git
   c646a65..aa74a2b  main -> main

compuni@Lab6m13 MINGW64 ~/AtividadeFinal (main)
$

- Criou o arquivo `algoritmo.por` com a estrutura inicial:
  programa {
  funcao inicio() {
    inteiro n1, n2
  }
}
  
- fez o que? depois?...
  Eu adicionei a variável n1 e n2 como inteiro no "algoritmo.por", salvei, dei um "git status" que mostrou arquivo modificado, depois um "git add ." para adicionar as modificações, em seguida dei um "git status" para verificar, depois um "git commit -m" com a descrição e por fim um "git push".

### Ciclana Souza
- Como Configurou o Git? não deixe exposto sua chave.
- Fez `git pull` após o commit de Fulano.
- Adicionou lógica de ... 
 

### Beltrano Gomes 
- Como Configurou o Git? não deixe exposto sua chave.
- Fez `git pull` após o commit de Ciclana.
- Finalizou o algoritmo com lógica . . .


## Comandos utilizados
Todos os comandos foram executados via terminal utilizando chave SSH:
### Comandos de Fulano
- git status
- git add .
- git commit -m
- git push
### Comandos de Ciclana

### Comandos de beltrano

## Observações
Cada etapa foi realizada por apenas um integrante por vez, primeiro o João Victor, depois o Fernando e Pietro, respeitando a ordem de commits e a integridade do código.
