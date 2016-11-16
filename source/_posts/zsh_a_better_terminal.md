---
layout: post
title: Zsh - A Better Terminal
tags:
- Terminal
- Zsh
categories:
- Tutorials
---

## What is Zsh and why should you care?
Zsh features themes, plugins, and advancements over default Bash and is compatible. But to put it frankly:

> IT WILL MAKE THE TERMINAL EASY AND FUN TO USE.

![](/images/zsh_example.png)

The following is a concise guide on how to get up and running with this powerhouse of a tool.

<!-- more -->

### Skip to Sections:
- [What is Zsh and why should I care?](#zsh_sec1)
- [HOW DO I GET THIS NOW](#zsh_sec2)
- [Oh-My-Zsh](#zsh_sec3)
- [Making it Awesome](#zsh_sec4)
- [Resulting Workflow](#zsh_sec5)


## How to Install: <a name="sec1"></a>

1. Install with the package manager of your choice. Ex:
```bash
$ sudo apt-get install zsh)
```
2. Verify installation by running:
```bash
$ zsh --version # Expected result: zsh 4.3.9 or more recent.
```
3. Make it your default shell:
```bash
$ chsh -s $(COPY_VERSION_OUTPUT_HERE) # Ex: chsh -s $(zsh 4.3.9)
```
4. Log out and log in again to your terminal and test that it worked:
```bash
 $ echo $SHELL # Expected result: /bin/zsh  
```

For more information/troubleshooting:  
https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH

## Oh-My-Zsh - A Must Have <a name="sec2"></a>
‘Oh My Zsh is an open source, community-driven framework for managing your zsh configuration.’

(It makes it awesome.)

To install, run the following:

via curl:
```bash
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Or via wget:
```bash
  sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

## Making it Awesome with Themes and Plugins and Fonts!<a name="sec3"></a>

### Themes

To configure your zsh, modify the ‘.zshrc’ file in your home directory. Example:   nano ~/.zshrc
NOTE: Whenever you make changes to the config file, in order to update terminal, run:   source ~/.zshrc
> Enabling Themes  

Modify the ZSH_THEMES line of  ‘.zshrc’.  Example: ZSH_THEME="agnoster"
If you’re looking to try a new theme every time you can use: ZSH_THEME="random"

### Plugins

Enabling Plugins
Modify the plugins line of  ‘.zshrc’. You can add any available plugins. Example: plugins=(git node npm wd)

For a list of bundled plugins: https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins

REMEMBER: Whenever you make changes, run:   source ~/.zshrc


### Fonts

In order to realize the full awesomeness, you’re going to need some new fonts, you can download them from here:
https://github.com/powerline/fonts
Once installed, you can select them in terminal preferences as shown to the right.

### Results
