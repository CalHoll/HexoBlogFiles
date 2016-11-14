---
title: Migrated blog to Hexo, workflow and quick-refs:
---

Hexo Documentation: [documentation](https://hexo.io/docs/) 


## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

The following script currently has issues. To deploy I have created an upstream from the public folder. 
Simply generate new static files, navigate into the public folder, and git push origin master.

Pro Tip - to overwrite git remote files include a "+" before remote branch like so:  git push origin +master

``` bash
$ hexo deploy
```


More info: [Deployment](https://hexo.io/docs/deployment.html)
