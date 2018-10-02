## Pull

```sh
git status
# if you have changes
git stash

git pull --rebase
# or 
git pull --rebase <remote> <branch>

git stash pop
```

## Stash

```sh
git stash list
git stash show -p
git stash show -p stash@{1}
```

## Git tree

This is not native command

```sh
git log --graph --decorate --pretty=oneline --abbrev-commit
```
Add this permanently to git config
```sh
git config --global alias.tree "log --graph --decorate --pretty=oneline --abbrev-commit"  
```
```sh
git tree
```
