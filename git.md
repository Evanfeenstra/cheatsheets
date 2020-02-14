# git

### basic 

`git init`: starts a git project in your current directory

`git add .`: add all your changes to git

`git commit -m "message"`: commit you changes

`git remote add origin https://...`: link your project to a repo on github (you can copy this line from github after creating the repo)

`git push origin master`: push to github

`git status`: check which files have changed

note: the `.gitignore` file lets you add "ignored" files and directories. ALWAYS add "node_modules" to `.gitignore`

### cloning

`git clone https://...`: clone someone else's repo

`git remote set-url origin https://...`: to change the remote URL to your own github repo

### merging

`git checkout -b branch-name`: make a new branch

`git merge branch-name`: merge your current branch with branch-name

### pulling

`git pull origin branch-name`: pull from github