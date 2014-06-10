# Git

## Configurations

enable colored text output

    git config --global color.ui true
  
set user variables

    git config --global user.name 'Everton R. Auler'
    git config --global user.email 'example@gmail.com'
    
some interest command to show the project log

    git config --global alias.lol 'log --graph --decorate --pretty=oneline --abbrev-commit --all'
    
use it

    git lol
    
## Using Git
Initialize project

    cd project/path/
    git init		# creates a .git/ folder
    
Adding files to stagging area

    git add . --all     # all files
    git add folder		# a folder
    git add file.html	# a file
    
Show status

    git status
    
First commit

    git commit -m 'commit inicial'	
    
Create a branch

    git checkout -b 'branch_A'

Show all the branchs

    git branch
    
switch branch (to branch 'master')

    git checkout master
    
show the diff

    git diff
    git diff --word-diff
    
commit using just a command

    git commit -am 'I changed the background color'

Using merge (branch 'master', master = master + branch_A)

    git merge branch_A

Using rebase (branch 'master', master = master + branch_A)

    git rebase branch_A

Using clone

    git clone https://github.com/evertonrobertoauler/fenalivre.git

Reset all modification

    git reset --hard

Create a tag locally and remotely

    git tag v1.0
    git push origin v1.0
    
Move HEAD to a tag

    git checkout v1.0
    
Delete a tag locally and remotely

    git tag -d v1.0
    git push origin :refs/tags/v1.0
