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
 git branch -d  (delete branch)
 
 3 way merge vs fast foward merge
 
 git switch --detach abc123 
 git stash list -p
 
 git log = git history git log --all --decorate --oneline --graph = commit history graph 
 git branch (branch-name) = create a branch git checkout (branch-name) = checkout a branch/move head pointer 
 git commit -a -m "commit message" = commit all modified and tracked files in on command (bypass separate 'git add' command) 
 git diff master..SDN = diff between 2 branches git merge (branch-name) = merge branches (fast-forward and 3-way merges) 
 git branch --merged = see branches merged into the current branch 
 git branch -d (branch-name) = delete a branch, only if already merged 
 git branch -D (branch-name) = delete a branch, including if not already merged (exercise caution here) 
 git merge --abort = abort a merge during a merge conflict situation git checkout (commit-hash) = checkout a commit directly, not through a branch, results in a detached HEAD state 
 git stash = create a stash point 
 git stash list = list stash points 
 git stash list -p = list stash points and show diffs per stash git stash apply = apply most recent stash 
 git stash pop = apply most recent stash, and remove it from saved stashes 
 git stash apply (stash reference) = apply a specific stash point git stash save "(description)" = create a stash point, be more descriptive