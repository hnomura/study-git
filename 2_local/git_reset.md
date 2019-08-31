## git reset 

### Unsage, but keep changes in working area
```
$ git reset [<file-spec>]
```
> $ git add some-file   
> $ git reset some-file 

```
$ git reset [commit(HEAD when omitted)]
```

### Unstage & revert changes in working area : Revert to latest commit 
```
$ git reset --hard [commit(HEAD when omitted)]
```
NOTE: This throws away all changes made in working area.  Be careful.  

### Revert to latest commit, do not change staging & working area
```
$ git reset --soft [commmit]
```
Typical usege will be similar to `commit --amend` to modify latest commit as follows. 
With `--soft` with `HEAD~`, the content of `HEAD` will be in staging area.  
Commot can be modified with other files added, etc.  
> $git reset --soft HEAD~
> $git commit


