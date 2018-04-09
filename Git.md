# Git commands

## Create
1. `$git init` - create a new local repository
1. `$git clone <repo.git>` - clone an existing repository

## Local changes
1. `$git status` - shows changed files in the local repository
1. `$git add .` - add all current changes to the next commit
1. `$git commit -m "comment"` - commit previously staged changes

## Branches and tags
1. `$git branch -av` - list all current branches
1. `$git checkout <branch>` - switch head branch
1. `$git branch <new branch>` - create new branch based on your current head
1. `$git branch -d <branch>` - delete a local branch

## Update and Publish
1. `$git pull <remote> <branch>` - download changes from remote and directly merge into the head
1. `$git push <remote> <branch>` - publish local changes to the remote repo
1. `$git remote -v` - list currently all configured remotes
1. `$git branch -dr <remote/branch>` - delete a branch on the remote

## Merge and Rebase
1. `$git merge <branch>` - merge branch into your current head
1. `$git rebase <branch>` - rebase your current head onto branch


