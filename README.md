#Resumo de Git

##Configurações do Git

texto colorido

  git config --global color.ui true
  
setar variáveis para historico

    git config --global user.name 'Everton R. Auler'
    git config --global user.email 'evertonrobertoauler@gmail.com'
    
criar um comando (git lol)

    git config --global alias.lol 'log --graph --decorate --pretty=oneline --abbrev-commit --all'
    
##Usando Git
cria repositório

    cd projeto/
    git init		# cria pasta .git/
    
adiciona o que sera feito commit

    git add .		# todos os arquivos
    git add foler		# uma pasta
    git add file.html	# um arquivo
    
ver o status, caso tenha algo modificado ou novo sera listado

    git status
    
commit do que foi feito add

    git commit -m 'commit inicial'	
    
criar novo branch para fazer uma tarefa

    git checkout -b 'branch_A'

para ver lista de branches

    git branch
    
para trocar de branch (para o branch 'master')

    git checkout master
    
ver modificações do branch atual, que não foi feito commit

    git diff
    git diff --word-diff
    
fazer o commit sem precisar dar git add

    git commit -am 'mudei a cor para vermelho'

usando merge de branch (branch atual 'master', master = master + branch_A)

    git merge branch_A

usando rebase de branch (branch atual 'master', branch_A = master + branch_A)

    git rebase branch_A

usando clone

    git clone https://github.com/evertonrobertoauler/fenalivre.git

voltar branch ao estado do ultimo commit

    git reset --hard
