---
title: "How I Deployed This Site to Github"
date: 2024-01-14T13:25:26+01:00
draft: true
toc: false
author: 
  name: radopeti
images:
tags: [ "github", "hugo" ]
---

## Quick introduction
This is a step by step tutorial how to deploy a **Hugo** website to **{user}.github.io**

These are the steps I followed:

1. **follow** the [quickstart guide](https://gohugo.io/getting-started/quick-start/) and add the template you find the best for your interest
2. **init** your local github repo
3. **create** a repo on **github** with name like: **{user}.github.io** and push your local repo 
4. **go** to your **repo settings** on github and do the following:
  ![github pages settings](/how-i-deployed-this/build-and-deploy.png)
5. **set** the **publishDir** variable to **docs** in **hugo.toml** (_running hugo command will put all the generated files into this dir because the setting above expects /docs as the publish dir_)
6. **commit** and **push** the changes, this will trigger to build and deploy automatically
7. **visit** _{user}.github.io_

#### Enjoy your site!
