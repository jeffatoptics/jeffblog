---
title: 关于网站笔记 jekyll 和 mkdocs
layout: post
category: work
tags:
author: 
- jeffatoptics
created: 2022-04-29 Fri-13:00
---

Github page 发日记可以有三个方法:

-在本地完成Markdown，生成html文件。然后直接push到Github项目目录里。这样写单个文件方便，但是做多个文件链接时，需要特意处理一下。

- 在本地完成Markdown，直接push到Github项目里，Github的jekyll 会基于缺省或者选择的 theme,把 markdown 文件转成html. 
    - 好处: 方便，多个文件很容易自动被index page做链接根据时间，或者tag分类发表(如jekyll_posts目录的markdown文件)
    - 坏处: 有些特殊的markdown插件语法可能在 jekyll 行不通。jekyll 的_posts目录的链接方式也比较怪异，有时候索引文件需要需要用到jekyll定义的网站变量

- 在本地完成Markdown，然后采用 [mkdocs](https://www.mkdocs.org/) 或者[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)，直接生成site html文件。然后把site文件push上去。

以后关注学习一下 [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)。感觉功能很强大。

---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](2022-04-28-late-night.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next](2022-04-29-mpe-inline-code.md)

---
