---
title: "How I Deployed This to Github"
date: 2024-01-14T13:25:26+01:00
draft: true
toc: false
author: radopeti
images:
tags:
---

# How to deploy a Hugo website to

## Quick introduction
This is a step by step tutorial how to deploy a Hugo website to {user}.github.io

These are the steps I followed:

1. follow the quickstart guide and add the template you find the best for your interest
2. init your local github repo
3. create a repo on github with name like: {user}.github.io and push your local repo 
4. go to your repo settings 
![github pages settings](/how-i-deployed-this/build-and-deploy.png)
5. set the publishDir variable to docs in hugo.toml (running hugo command will put all the generated files into this dir because the setting above expects /docs as the publish dir)
6. commit and push the changes, this will trigger to build and deploy automatically
7. visit {user}.github.io

Enjoy your site!
