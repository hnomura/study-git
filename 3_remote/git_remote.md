## git remote 

### add remote 
```
$ git remote add <remote_name> <remote_repo_url>
```

> $ git remote add origin https://github.com/hnomura/my_repo.git

### push to remote 
```
$ git push -u <remote_name> <branch_name>
```

> $ git push -u origin master 

### set as tracked remote branch 
```
$ git push --set-upstream <remote_name> <branch_name> 
```
> $ git push --set-upstream origin master 

Current local branch points to the specified remote branch by default.  
No need to specify name/branch to `git push`, `git pull`, etc. 

### Checkout remote branch to local as tracked branch
```
$ git checkout -b <branch_name>  <remote_name>/<branch_name>
```

> $ git checkout -b branch_x   origin/branch_x 


