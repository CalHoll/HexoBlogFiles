---
layout: post
title: Introductions & Why I Chose a Hexo Blog
---

Hello and welcome to my new site using github pages and Hexo.  I am a current student of Hack Reactor Remote, cohort 20, and am absolutely thrilled to be diving into the world of Software Engineering!  

My time at Hack Reactor will be a unique opportunity to experience what it is like to make a shift from Mechanical Engineering to Software Engineering, or a combination thereof.

The purpose of this blog will be to share knowledge and resources that I find particularly interesting, to hopefully assist those who are also trying to get involved.

----

## Why I Chose Hexo

In the interest of jumping right in, I want to share what has helped me get my site here up and running.

>>DOUBLENOTE: For those looking for an in depth guide I would recommend the tutorial found here:   [Build A Blog With Jekyll And GitHub Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/)

---


### My site is live... now what?

I wanted to compile a few 'pro-tips' for anyone else that might be interested in how I made this page. Mostly this is just for my own selfish goal of learning by doing. BUT HERE THE TIPS ARE:

[You can view the markdown used to create this post(UNDER CONSTRUCTION)](https://raw.githubusercontent.com/barryclark/www.jekyllnow.com/gh-pages/_posts/2014-6-19-Markdown-Style-Guide.md)

Use three consequetive backticks within post Markdown (.md) files beforee and after javascript inline code snippets like so:

```javascript
var MyFavoriteClass = function() {
  // Can anyone guess this class instantiation style?
  this.idx = 0;
  this.storage = {};
};

MyFavoriateClass.prototype.addMethod = function(value) {
  this.storage[this.idx] = value;
  this.idx++;
};
```

### issues hosting Jekyll locally
This could be in part due to my choice to do all this on a Ubuntu box but...

When trying to run 'bundle exec jekyll serve', I got a funny error about not being able to install RedCloth. Apparently I needed the 'dev' version of ruby, install command follows:  

> $ sudo apt-get install ruby-dev

Also had issues with "gem install nokogiri -v '1.6.8.1'", resolved those with:  
> $ sudo apt-get install zlib1g-dev

 &  
> $ sudo apt-get update  
> $ sudo apt-get install libxml2-dev  
> $ sudo apt-get install libxslt-dev  
> $ sudo gem install nokogiri -v '1.4.7'  


apt-get install ruby-dev
apt-get install libxslt-dev libxml2-dev
apt-get install zlib1g-dev
gem install nokogiri

$ gem list nokogiri
*** LOCAL GEMS ***
nokogiri (1.4.7)

### List of Jekyll console commands to remember:

Jekyll --help
:satisfied:

### Jekyll emoji plug-ins?!

After a little madness working with local Gemfiles...
I give this plugin two :+1:!  

Emoji reference here: [Emoji Cheat Sheet](http://www.webpagefx.com/tools/emoji-cheat-sheet/)  

A couple to get you started:
(place words between two ':')  
fire:fire:  
smile:smile:  
grin:grin:  
joy:joy:  
laughing:laughing:  

#### Stay tuned for more!



## Migrated blog to Hexo, workflow and quick-refs:

Hexo Documentation: [documentation](https://hexo.io/docs/)


[CREATE AN HEXO THEME](http://www.codeblocq.com/2016/03/Create-an-Hexo-Theme-Part-1-Index/)


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
