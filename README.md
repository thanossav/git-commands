## 1. Remotes

### List the current remotes associated with the local repository
```
git remote -v
```

### Add a remote
```
git remote add [name] [URL]
```

### Remove a remote
```
git remote remove [name]
```

### Fetch a remote
> Downloads objects and refs from a remote
```
git fetch [remote]
```


### -----------------------------------------------------------------------------------------------------------------------------


## 2. Branches


### List local branches
```
git branch
```


### List all branches
```
git branch -a
```


### Move to a specified branch
```
git checkout [branch-name]
```


### Create a branch and then move to it
> Shortcut for ```git branch [branch-name]``` ```git checkout [branch-name]```
```
git checkout -b [new-branch-name]
```


### Create a new orphan branch from checked-out branch
> Removes all tracking history
```
git checkout --orphan [new-branch-name]
```


### Delete a local branch
> First checkout to master or any other branch except the one that is being deleted
```
git checkout master
git branch -D [branch-name]
```


### Delete a remote branch
```
git push [remote] --delete [branch-name]
```


### Push checked-out branch to a remote
> Destination branch will have the same name as [branch-name]
```
git push [remote] [branch-name]
```


### Push checked-out branch to another branch on a remote
```
git push [remote] [source_branch]:[destination_branch]
```


### Fetch a remote branch to local machine
> git switch creates local branch with the same name as remote branch and sets upstream

> shortcut for ```git checkout --track [remote]/[remote-branch]``` 

> which is a shortcut for ```git checkout -b [local-branch] [remote]/[remote-branch]```
```
git switch [remote-branch]
```







