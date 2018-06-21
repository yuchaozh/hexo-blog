---
title: Preview Git Stash Content
date: 2018-06-20 16:59:57
tags: Git
---

If you want see the preview of your git stash content without applying them. You can use `git stash show` command to do so.

### preview the content of the most latest stash

```
git stash show -p
```

### preview specific stash content

```
git stash show -p stash@{i}  
```

### only want to know names of stash files
```
git stash show -p stash@{i} --name-only
```


More Information: [See what's in a stash without applying it](https://stackoverflow.com/questions/10725729/see-whats-in-a-stash-without-applying-it)