+++
date = 2017-05-31
lastmod = 2017-10-15
draft = false
tags = []
title = "Move to Hugo"
math = true
summary = """
Move to Hugo
"""
+++

## Intro
I have moved my homepage to [Hugo](https://gohugo.io/) which I think is the fastest static website generator. 
On the other hand, I like the theme - [Acadmic](https://github.com/gcushen/hugo-academic) which is best for the persons who like me is in academia. 


However, there is one problem that Hugo can not be automatically generated as Jekyll in Github Page. 
I referred to the solution which is provided by the author of Acadmic [^1] to use [Wercker](http://www.wercker.com/) to automatically generate the pages from source files to HTML. 
The processes are as below.

<!--more-->

## Setup Website
You need to firstly setup a hugo website, test it locally and upload to one of your github repositories. 
I assume the repository is [`homepage`](https://github.com/xujinlai/homepage).

## Create Personal Website Repository
I use [`xujinlai.github.io`](https://github.com/xujinlai/xujinlai.github.io) as the personal website repository.

## Setup Wercker
You can treat Wercker as an automatically builder which can build your website imediatly after you push your update with git.

It is also very easy to use, which you just need to setup an application on [Wercker](http://www.wercker.com/) with logining wity your Github account. You just need to follow the instruction below to setup the automatically builder for your website:

 1. Login to [Wercker](http://www.wercker.com/) with your github account such as [Jinlai Xu](https://github.com/xujinlai).
 2. Add an application and setup the repository of the application to `homepage`.
 3. Add an `wercker.yml` file in your repository for example [Wercker.yml example](#wercker-yml-example)
 4. You need to modify the above `wercker.yml` with your own `repo` name and your own `domain` name.
 5. Add a `$GIT_TOKEN` parameter in your wercker application to make it possible to access your github repositories. You can refer to [^2] to get the details.
 6. Add a `deploy` step after `build` step in your wercker application's `Workflows` page.
 7. Upload you website to `homepage` to test if your wercker application is automatically run.

## Wercker.yml example
```yaml
box: golang

build:
  steps:
    - add-to-known_hosts:
        hostname: github.com
        fingerprint: 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48
        type: rsa
    - script:
        name: initialize and update git submodules
        code: |
            git submodule init
            git submodule update --remote --recursive
    - arjen/hugo-build:
        version: "0.20.7"

deploy:
  steps:
    - lukevivier/gh-pages:
        token: $GIT_TOKEN
        basedir: public
        repo: xujinlai/xujinlai.github.io
        domain: jinlaixu.net
```

[^1]: [Create a Free Personal Academic Website with Hugo](https://georgecushen.com/create-your-website-with-hugo/#automating-deployment)
[^2]: [Creating a personal access token for the command line](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/)
