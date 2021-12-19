=====================================================================================

# CREATE a new repository on the command line

=====================================================================================
- echo "# quotes-scrapy-bot" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin https://github.com/jdandridge/quotes-scrapy-bot.git
- git push -u origin main
=====================================================================================

# PUSH an existing repository from the command line

=====================================================================================
- git remote add origin https://github.com/jdandridge/quotes-scrapy-bot.git
- git branch -M main
- git push -u origin main
=====================================================================================

# GIT COMMANDS

=====================================================================================
- git --help
- git log --oneline
- git add .
- git push origin master
- git push origin main
- git push branch {branch name}
- git push --all branch
- git remote -V
- git remote remove origin
- git remote add origin {github repo url}
- git remote add branch {github repo url}

### When you already have a repo clone to computer

- git clone https://github.com/jdandridge/quotes-scrapy-bot.git
=====================================================================================

# Branches

=====================================================================================

## Create a branch

- git branch {name of your branch} ex: git branch new-feature

## Check all branches

- git branch -a

## Change into branch

- git checkout {branch name} ex: git checkout master-2
- git checkout master

## Delete / Make sure to be on master to delete others

- git branch -D new-feature
=====================================================================================

# MERGING

=====================================================================================

## Make sure you are on the master to merge other branches

- git checkout master
- git merge new-feature
=====================================================================================

# DELETE A COMMIT

=====================================================================================
- git reset --hard HEAD~2 -MORE THEN 1 COMMIT
- git reset --hard HEAD^ -FOR 1 COMMIT
=====================================================================================

# REMOVE GIT

=====================================================================================
- rm -rf git
