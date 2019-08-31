## git diff

### git diff 


***(1) Modified, not staged***  
What would be staged when `git add -u` next time?   
Note that this won't do nothing to newly created file.  
```
$ git diff [<file_path>]             # a/staged,           b/work-area
```

***(2) What will be committed next? *** 
```
$ git diff --cached [<file_path>]    # a/repo HEAD,       b/staged 
```

***(3) Changes made since latest commit ***
``` 
$ git diff HEAD  [<file_pagh>]       # a/repo HEAD,        b/work-area
```

***(4) Changes between two commits *** 
```
$ git diff <commit1>..<commit2>      # a/commit1,          b/commit2
```
> $ git fetch 
> $ git diff HEAD..FETCH_HEAD

***(5) 3-way diff fromm common ancestor ***
```
$ git diff <commit1>...<commit2>
```
