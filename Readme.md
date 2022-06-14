Conceitos

git - é uma sistema de versionamento capaz de suportar vários desenvolvedores 
      trabalhando no mesmo projeto. 

branch
    - é o conceito central para entendermos como trabalhar com git.
    - branch é um ramo, filial, sucursal, agência etc. 
    - exemplo: main, Master, Develop, meuProjeto etc. 


--- Master -----------o--------------------------------
   -
    -                                 
      - Develop -----o--------o-------
        -
          - minha-tela ----------------o   
            -
              ------- nova-funcionalidade ---------------


merge 
   - junção da branchs 

remote 
   - faz a ligação do meu repositório local, o repositório da minha 
     máquina, com o repositório do github 

push
   - empurra o que você fez na sua máquina para repositório 

pull
   - puxa o que esta no repositório para a sua máquina 

Histório do momento de cada comando


Você esta trabalhando no seu computador e salvando nos seus arquivos. 
   - file / save all 
          / save as 
          / save  

Você esta trabalhando no seu computador e vai transferir sua funcionaliade 
para uma Branch. Para criar uma Branch você precisa do Github. 

Baixar em http://github.com 

Após instalar: ver a versão no terminal do git com:
>git --version 
 
Vai aparecer algo parecido com:
PS C:\Users\Jackson Borges\Documents\ProjetoGit> git --version
git version 2.34.0.windows.1
PS C:\Users\Jackson Borges\Documents\ProjetoGit> 

Agora vamos criar a nome da Branch que onde você vai trabalhar:

>git init nome-da-branch 

Exemplo:

>git init desenv

Vai aparecer algo parecido com:
PS C:\Users\Jackson Borges\Documents\ProjetoGit> git init desenv
Initialized empty Git repository in C:/Users/Jackson Borges/Documents/ProjetoGit/desenv/.git/
PS C:\Users\Jackson Borges\Documents\ProjetoGit> 

Agora vamos ver onde estamos de fato trabalhando:

git status
   - para ver em qual branch você esta
   - aqui vai mostrar que eu estou na branch main


   - ..... inicio 
   - ::::: fim 
.................................................................
Jackson Borges@DESKTOP-BMQR85M MINGW64 ~/Meus Documentos/ProjetoGit (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Readme.md

no changes added to commit (use "git add" and/or "git commit -a")
:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

O comando git status mostra que Jackson esta na branch main, ele deu 
este nome para a branch.
A origem é a origin e vai para main. 
Tem um arquivo modificado que é o README.md
O github mostra que podemos add adicionar nossas modificações na branch main.
Como eu fiz alterações no arquivo README.md eu posso fazer uma commit na main.
Primeiro eu vou salvando as alterações na minha máquina.
Depois de uma periodo que achar apropriado eu faço o commit na main.
Deixando a main estável. 

Para mudar o nome da Branch para Develop:
>git branch -M "Develop"

Então temos o primeiro momento concluido. Eu faço as alterações no meu código 
e salvo na minha máquina e depois de um período eu faço commit -m na minha 
branch.  

Agora devemos fazer nossa conta no github e criar o repositório. 
Vamos agora fazer a conexão entre o minha máquina e o github.

>git remote add origin https://github.com.br/jacksonalencar/ProjetoGit

Pronto a conexão esta pronta. 


