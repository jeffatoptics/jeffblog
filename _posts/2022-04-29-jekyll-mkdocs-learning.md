---
title: 关于网站笔记 jekyll 和 mkdocs
layout: post
category: life
tags:
Author: 
- jeffatoptics
Created: 2022-04-29 Fri-13--00
---

Github page 发日记可以有三个方法:

- 本地Markdown写好，直接生成html文件。然后直接push到Github项目目录里。写单个文件方便，做多个文件连接时，链接需要特意处理一下。

- 本地Markdown写好，直接push到Github项目目录里，Github的会基于缺省或者选择的 jekyll theme,把mardown文件转成html. 
    - 好处：方便，多个文件很容易自动被index page做链接发表(如jekyll_posts目录)
    - 坏处 有些本地特殊的markdown插件语法可能行不通。jekyll的_posts目录的链接方式比较怪异，普通的markdown应用, html 链接语法有时对于非markdown文件，则行不通，需要用到jekyll定义的网站变量

- 本地Markdown写好，采用 [mkdocs](https://www.mkdocs.org/) 或者[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)，直接生成site html文件。然后把site文件push上去。

以后关注学习一下 [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)。感觉功能很强大。

- 
test absolute link in post folder ![](/assets/20220429/bird2.jpg)

---

[⏮️arrohome](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [ ◀️prev](2022-04-28-late-night.md) &nbsp; &nbsp; &nbsp; &nbsp; [ ▶️ next](2022-04-29-jekyll-mkdocs-learning.md)

---
