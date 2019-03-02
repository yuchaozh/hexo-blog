---
title: How to create a Hexo post
date: 2019-03-01 15:30:50
tags: Hexo  
---

### Clone the hexo-blog project to local
```
git clone https://github.com/yuchaozh/hexo-blog.git
```

### Install Hexo
```
npm install -g hexo-cli
```

### Init Hexo
go to the blog folder. e.g. `C:\Users\v-yuczh\Documents\GitHub\hexo-blog`
```
npm install
```

### Create a new post
```
hexo new "XXXXXXX"
```

### Turn up local server
```
hexo server
```
You can view your website locally at `http://localhost:4000`, you can check your new post locally.

### Deploy to prod 
```
hexo deploy
```

### Commit the changes to git
```
git add
git commit -m ""
git push
```

### Or Use hexo-deployer-git
```
npm install hexo-deployer-git --save
```
```
hexo clean && hexo deploy 
```
you have to use `clean && deploy` together. `hexo deploy` is not working anymore.
to deploy and commit to git at the same time. However, this will commit to `https://github.com/yuchaozh/yuchaozh.github.io` project, not the `hexo-blog` project. So you still need to commit to `hexo-blog` afater use the above command.