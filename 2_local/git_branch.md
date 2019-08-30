## git branch 

### list branch 
```
$ git branch               # local branches
$ git branch -r            # remote branches
$ git branch -a            # all branches 
```

### create breanch 
```
$ git branch <branch_name>       # create, but not to checkout 
$ git checkout -b <branch_name>  # create and checkout to the new branch 
```

### checkout existing branch 
```
$ git checkout <branch_name> 
```

### push to remote repository 
```
# pre-requisite 
$ git remote add <remote_name> <remote_repo_url>   # add remote

$ git checkout -b <branch_name>                    # prepare local branch
$ git commit                                       #  with commit(s) in it 

# push to remote 
$ git push -u <remote_name> <branch_name>
```

NOTE: `<remote_name> <branch_name>` must NOT be confused as `<remote_name>/<branch_name>`.   `git-push` allows to specify different branch name in remote by the following syntax.  
> $ git push <remote_name> <local_branch_name>:<remote_branch_name>

