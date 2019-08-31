## git remote 

### add remote 
```
$ git remote add <remote_name> <remote_repo_url>
```

> $ git remote add origin https://github.com/hnomura/my_repo.git

### push to remote 
```
$ git push <remote_name> <branch_name>
```

> $ git push origin master 

### set as tracked remote branch 
```
$ git push --set-upstream <remote_name> <branch_name> 
$ git push -u <remote_name> <branch_name>
```
> $ git push -u origin feature/f1_branch 

Current local branch points to the specified remote branch by -u (--set-upstream).  
No need to specify name/branch to `git push`, `git pull`, etc. 

### Checkout remote branch to local as tracked branch
```
$ git checkout -b <branch_name>  <remote_name>/<branch_name>
```

> $ git checkout -b branch_x   origin/branch_x 

### Delete remote branch 
```
$ git push --delete <remote_name> <branch_name> 
```

> $ git push --delete origin branch_name 

### Delete local branches already deleted on remote 
```
$ git fetch --prune 
```

> $ git branch -a       # list all branches 
> $ git fetch --prune   # delete branches already deleted on remote 

### Show remote 
```
$ git remote show <remote_name> 
```

> $ git remote show origin 


