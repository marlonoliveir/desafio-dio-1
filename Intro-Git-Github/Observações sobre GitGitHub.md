# Observações sobre Git/GitHub

 - Git e GitHub é um sistema de gerenciamento e armazenamento de arquivos/versões de arquivos que utiliza um prompt
de comando(Git Bash) para inserção, atualização e download de conteúdos e projetos.Possuindo tambem uma interface
gráfica e remota (GitHub).

 - O Git/GitHub utiliza três tipos de autenticação de autor/usuario antes de operar, elas são:

1. Autenticação por nome e senha usada para login no GitHub.

2. Autenticação por chave Token, veja como em (https://www.alura.com.br/artigos/nova-exigencia-do-git-de-autenticacao-por-token-o-que-e-o-que-devo-fazer)  

3. Autenticação por chave ssh (utilizada geralmente por dev´s em maquinas de uso comum).


 - Todo o comando que você precisar executar é necessario direciona-lo no Git Bash, isso só é possivel quando digitar
o comado com a palavra "git" antes.


 - Os commits tem a função de ostrar para a maquina o que foi alterado e o que ela deve executr, portanto antes de 
fazer uma importação da sua versão local para remota, obrigatóriamente todas as alterações devem ser informadas,
ou seja, "comitadas".Com base nisso você precisa estar ciente de duas termologias utilizadas para diagnosticar a 
situação do arquivo, elas são:

1. untraked = arquivos que o git não tem ciência (você não o informou "commit").

2. staged = arquivos que o git possui ciência e os commit´s estão devidamente feitos(Um arquivo pronto para ser executado).



 



#### Comandos Básicos Git Bash

1.cd = direcionar caminho para entrar em arquivos ou pastas

2.ls = listar arquivos e pastas

3.ls -a = mostrar pastas ocultas

4.mv = comando para mover arquivos entre pastas etc...

5.git init = iniciar um repositório

6.git config --global user.email"seu email" = comando para configurar inicialmente o Git e atribuir um autor aos commit´s que serão feitos.
                           name"seu nome de usuario no GitHub"

7.git add . ou * = comando para adicior um commit

8.git commit -m "texto informante"= comando para criar um commit

9.git satatus = usado para mostrar a situação dos arquivos/repositórios

10. git restore = usado para retirar arquivos da condição "staged"

11.git config --list = esse comando serve para listar as configurações do seu git, possiblitando o usuário confirmar a autenticidade do seus commit´s

12.git config --global --unset user.email = comando para alterar o autor dos commit´s
                                    name

#### Como adicionar e criar um commit

1.você irá alterar ou adicionar o arquivo que deseja na pasta aonde esta executando o seu Git Bash

2.no Git Bash digite o seguinte comando "git add ." para informar a alteração ou inclusão de um arquivo

3.no Git Bash digite o seguinte comando "git status" para a maquina mostrar se o arquivo ou alteração foi reconhecido.

4.no Git Bash digite o seguinte comando "git commit - m "texto"<- aqui voce desecreve o que fez.exemplo: inclusao de arquivo x"

5.no Git Bash digite o seguinte comando "git status" para verficar se o commit foi criado com sucesso, se sim, a mensgem dizendo que a arvore de trabalho esta limpa irá aparecer.



#### Como copiar um repositório do GitHub

1.escolha no GitHub um repositório que deseja e copie sua URL em Html

2.no Git Bash digite o seguinte comando "git clone" e a frente cole o link do repositório

3.uma mensagem dizendo que foi copiado com sucesso aparecerá.



#### Como tornar um repositório local em um remoto(importar)

1.no Git Bash digite o seguinte comando "git push (nome da branch)" 

2.se o comando tiver sucesso uma mensagem como essa vai aparecer:

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 466 bytes | 466.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/marlonoliveir/desafio-dio-1.git
   3a72af0..bb409ca  main -> main

3.caso não efetive a importação, verifique se há algum problema com o seguinte comando "git status" e o próprio Git irá propor uma solução.




​                                   