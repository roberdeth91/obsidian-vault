git init - initialize a new repo in a directory 
git config --global user.name "name" 
git config --global user.email "email"
git config --list
git status
git add 
git diff --staged

git switch main 
git restore --source=<hash-del-commit> s2 
git add s2 
git commit -m "Restaurar s2"
 git log --all --decorate --oneline --graph

git switch -c nueva` (o `checkout -b`) → crea la rama y te cambia a ella en un solo paso.

 git branch --merged (para ver que branches estan merged)