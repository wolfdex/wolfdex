git init

git add <FILE>
git add .

git commit -m 'COMMENT'
git commit -a -m 'COMMENT'

geänderte Dateien
git diff --name-status firstbranch..yourBranchName

einzelne Datei in Branch übernehmen
git checkout sourcebranch -- file

git pull --rebase

## rename master to main
### local
git branch -m master main

### remote
git push -u origin main
git push origin --delete master

###
git checkout master

git branch -m master main

get the latest commits and branches from the remote:
git fetch

Remove the existing tracking connection with "origin/master":
git branch --unset-upstream

Create a new tracking connection with the new "origin/main" branch
git branch -u origin/main


## Git Config (global)
git config --global user.name "User Name"
git config --global user.email "my@email"

## New Repository
### new Empty Project
git clone https://gitlab.com/<user>/<project>.git
cd <project>
git switch -c main
touch README.md
git add README.md
git commit -m "add README"
git push -u origin main

##new Empty Project, folder exists
cd <existing_folder>
git init --initial-branch=main
git remote add origin https://gitlab.com/<user>/<project>.git
git add .
git commit -m "Initial commit"
git push -u origin main

##existing git Project
cd <existing_repo>
git remote rename origin old-origin
git remote add origin https://gitlab.com/<user>/<project>.git
git push -u origin --all
git push -u origin --tags
