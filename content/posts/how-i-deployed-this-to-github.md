---
title: "How I deployed this site to my Github pages"
date: 2024-01-14T13:25:26+01:00
draft: false
toc: false
author: 
  name: radopeti
images:
tags: [ "github pages", "hugo", "tutorial" ]
---

## Quick introduction
This is a step by step tutorial how to deploy a **Hugo** website to **{user}.github.io**

### These are the steps I followed:

1. **follow** the [quickstart guide](https://gohugo.io/getting-started/quick-start/) and add the template you find the best for your interest. I use [hello-friend-ng](https://themes.gohugo.io/themes/hugo-theme-hello-friend-ng/).
2. **init** your local github repository
3. **create** a new repository on **github** with name like: **{user}.github.io** and push your local repo 
4. **go** to the **repository settings** on github and setup the build:
  ![github pages settings](/how-i-deployed-this/build-and-deploy.png)*(this means every push to master will trigger a build using the docs folder as source)*
5. **set** the **publishDir** variable to **docs** in **hugo.toml** (_running hugo command will put all the generated files into this dir because the setting above expects /docs as the publish dir_)
6. run 
    ```console
    foo@bar:~$ hugo
    ````
7. **commit** and **push** the changes, this will trigger the **pages-build-deployment** workflow
8. **visit** _{user}.github.io_ when the workflow run is completed

#### Enjoy your site!
