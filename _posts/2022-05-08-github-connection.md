---
title: 连接Github
layout: post
category: coding
author: jeffatoptics
created: 2022-05-08 Sun 13:43
modified_date:
---

[Gighub520](https://github.com/521xueweihan/GitHub520)提供了HOSTS的实时更新，把里面的内容直接COPY到本地电脑的文件后，访问竟然非常流畅。

1. `command` ➡`run as administrator`
1. `C:\WINDOWS\system32>cd drivers\etc`
1. `C:\WINDOWS\system32>cd drivers\etc>notepad hosts`

[faster-hosts](https://github.com/gauseen/faster-hosts)基于[Gighub520](https://github.com/521xueweihan/GitHub520)的HOSTS文件提供了插件。我在VPN和没有VPN的环境上各自试了一下插件，访问github普通文件都可以，但是没有VPN的环境下，图片相关的网址`raw.githubusercontent.com`访问不了, 手工设置hosts的ip没有问题，应该是插件问题。

---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](./2022-05-07-zettelkasten-book-reading.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
