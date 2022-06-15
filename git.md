git init

git add <FILE><br>
git add .

git commit -m 'COMMENT'<br>
git commit -a -m 'COMMENT'

geänderte Dateien<br>
git diff --name-status firstbranch..yourBranchName

einzelne Datei in Branch übernehmen<br>
git checkout sourcebranch -- file

git pull --rebase

## rename master to main
### local
git branch -m master main

### remote
git push -u origin main<br>
git push origin --delete master

###
git checkout master

git branch -m master main

get the latest commits and branches from the remote:<br>
git fetch

Remove the existing tracking connection with "origin/master":<br>
git branch --unset-upstream

Create a new tracking connection with the new "origin/main" branch<br>
git branch -u origin/main


## Git Config (global)
git config --global user.name "User Name"<br>
git config --global user.email "my@email"

## New Repository
### new Empty Project
git clone https://gitlab.com/&lt;user&gt;/&lt;project&gt;.git<br>
cd ;project&gt;<br>
git switch -c main<br>
touch README.md<br>
git add README.md<br>
git commit -m "add README"<br>
git push -u origin main

## new Empty Project, folder exists
cd <existing_folder><br>
git init --initial-branch=main<br>
git remote add origin https://gitlab.com/&lt;user&gt;/&lt;project&gt;.git<br>
git add .<br>
git commit -m "Initial commit"<br>
git push -u origin main<br>

## existing git Project
cd &lt;existing_repo&gt;<br>
git remote rename origin old-origin<br>
git remote add origin https://gitlab.com/&lt;user&gt;/&lt;project&gt;.git<br>
git push -u origin --all<br>
git push -u origin --tags
