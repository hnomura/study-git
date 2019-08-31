## git checkout 
Basically, all of the following changes files in working area. 
The source to use for the change is different.  

### Checkout from Branch 
```
$ git checkout <branch_name>
```
> $ git checkout develop 

### Checkout from specific commit 
```
$ git checkout <commit> 
```
> $ git checkout                     # change working area to the latest HEAD 
> $ git chekcout HEAD~               # change working area to the parent of the latest HEAD 
> $ git checkout HEAD~  file_spec    # do it to a specific file only 

### Checkout to create new branch 
```
$ git checkout -b <new_branch_name>   # branch from currently selected branch 
# git checkout -b <new_branch_name> <from_branch_name> 
```
> # create new feature branch locall, from the currently selected branch 
> $ git checkout -b feature/new_function  

> # create new tracked branch from the existing remote branch 
> $ git checkout -b feature/new_function origin/feature/new_function




