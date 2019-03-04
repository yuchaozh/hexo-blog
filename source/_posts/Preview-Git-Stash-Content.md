---
title: Git Stash
date: 2018-06-20 16:59:57
tags: Git
---

If you want see the preview of your git stash content without applying them. You can use `git stash show` command to do so.

### Preview the content of the most latest stash

```
git stash show -p
```

### Preview specific stash content

```
git stash show -p stash@{i}  
```

### Only want to know names of stash files
```
git stash show -p stash@{i} --name-only
```

### Stach untracked new files
By default, `git stash` only stash tracked files. It will not stash new created files which are untracked.
```
git stash --all
```


More Information:   
[See what's in a stash without applying it](https://stackoverflow.com/questions/10725729/see-whats-in-a-stash-without-applying-it)  
[How do you stash an untracked file?](https://stackoverflow.com/questions/835501/how-do-you-stash-an-untracked-file)