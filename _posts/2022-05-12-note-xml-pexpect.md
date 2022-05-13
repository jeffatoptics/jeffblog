---
title: xml 及pexpect以及其它
layout: post
category: coding
author: jeffatoptics
created: 2022-05-13 Fri 01:17
modified_date:
---

这两天忙着支持网管的接口。做一些结果记录时候，发现 markdown 笔记 code 标识里<kbd>```xml</kbd>加上 xml 后，结果显示清爽了很多. 

```xml
<hello xmlns="urn:ietf:params:xml:ns:netconf:base:1.0">
<capabilities>
<capability>urn:ietf:params:netconf:base:1.0</capability>
</capabilities>
</hello>
```
另外考虑做一下 Automation 的任务，看了一下几个选择, 也尝试了一下，准备基于 paramiko 做些东西.
比较怀念以前用的 procomm 的 terminal ，在上面能快速开发做一些界面和脚本。调试很方便，随时介入.

- [pexpect](https://pexpect.readthedocs.io/en/stable/): 对于windows支持不是很给力。

    - 子模块 [popen_spawn](https://pexpect.readthedocs.io/en/stable/api/popen_spawn.html) 是给 windows spawn 用的。简单尝试了一下，进入linux后，发现buffer里有时候没有抓住内容。
    - ssh输入password 无法交互，用了 `ssh -t -t` 后勉强能用，但需要手工自己输入密码。

- [winexpect](https://github.com/geertj/winpexpect) 2011年后 没有更新

- [wexpect](https://github.com/raczben/wexpect) 情况好些，以后备用

- [paramiko](https://github.com/paramiko/paramiko) 基础功能强大

- [paramiko-expect](https://github.com/fgimian/paramiko-expect) 看着似乎很好用，下一步试一下.

---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](./2022-05-08-summer-coming.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
