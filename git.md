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
