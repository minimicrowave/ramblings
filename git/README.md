# Git Notes

## Branching

### To update the local list of remote branches
`git remote update origin --prune`

### To show all local and remote branches that (local) Git knows about
`git branch -a`


## Credentials

### Prevent repo from using git store credentials
`git config --local credential.helper ""`


## Logging

### Visualise commits with branches
`git log --oneline --graph`


## Stashing

### Stash outstanding changes 
`git stash`


### List stashes
`git stash list`


### See specific item in stack
`git stash show -p "stash@{3}"`


### Applies changes and leaves a copy in stash
`git stash apply stash@{3} || STASH-NAME`

### Applies changes and removes files from stash
`git stash pop stash@{3} || STASH-NAME`