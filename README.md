# Como é o fluxo de utilização do Git / GitHub


## Fluxo de trabalho Git local

01. git checkout -b (nome-da-branch) Cria uma nova branch e já ativa
02. cria ou atua arquivos
03. git status
05. git add *arquivos*'
06. git status
07. git commit -m "minha mensagem"
08. git checkout main (mudando para a branch principal)
09. git merge nova_branch

## Fluxo de trabalho GitHub <> Local (projeto próprio ou da sua empresa)
01. git clone (endereco do projeto)
02. git checkout -b <nova_branch>
03. alterações de arquivos
04. git status
05. git add *arquivos*
06. git status
07. git commit -m "nova mensagem"
08. git push origin (nova_branch)
09. abrir Pull request no GitHub para main
10. git branch -D excluir "nova_branch" origin
11. git checkout main
12. git branch -D (nova_branch)

## Fluxo de trabalho GitHub <> Local (projetos open-source)
01. Fork do projeto para seu próprio github
02. git clone (endereco do projeto fork)
03. git checkout -b (nova_branch)
04. alterações de arquivos
05. git status
06. git add *arquivos*
07. git status
08. git commit -m "nova mensagem"
09. git push origin (nova_branch)
10. abrir Pull request no GitHub da branch fork para a main do projeto original
11. excluir (nova_branch) origin
12. git checkout main
13. git branch -D (nova_branch)

## Para excluir um Branch local e remota
git branch -D nomeDoBranchLocal


## Tipo e descrição de commits

# feat
  >> Commits do tipo feat indicam que seu trecho de código está incluindo um novo recurso (se relaciona com o MINOR do versionamento semântico).

# fix 
  >> Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix), (se relaciona com o PATCH do versionamento semântico).

# docs
  >> Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).

# test
  >> Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)

# build
  >> Commits do tipo build são utilizados quando são realizadas modificações em arquivos de build e dependências.

# perf
  >> Commits do tipo perf servem para identificar quaisquer alterações de código que estejam relacionadas a performance.

# style
  >> Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons, trailing spaces, lint... (Não inclui alterações em código).

# refactor
  >> Commits do tipo refactor referem-se a mudanças devido a refatorações que não alterem sua funcionalidade, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review.

# chore
 >> Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)

# ci
  >> Commits do tipo ci indicam mudanças relacionadas a integração contínua (continuous integration).

# raw
  >> Commits do tipo raw indicam mudanças relacionadas a arquivos de configurações, dados, features, parâmetros.

# cleanup
  >> Commits do tipo cleanup são utilizados para remover código comentado, trechos desnecessários ou qualquer outra forma de limpeza do código-fonte, visando aprimorar sua legibilidade e manutenibilidade.

# remove
  >> Commits do tipo remove indicam a exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas, reduzindo o tamanho e a complexidade do projeto e mantendo-o mais organizado.
>  
# Exemplo Utilização
  >> git add .
  >> git commit -m "feat: adicionar funcionalidade xyz"



#Parte do Texto retirado da live do @TeoMeWhy
