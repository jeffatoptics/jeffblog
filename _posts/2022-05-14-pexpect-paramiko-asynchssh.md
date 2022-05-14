---
title: pexpect paramiko asynchssh 及其它
layout: post
category: coding
author: jeffatoptics
created: 2022-05-14 Sat 12:27
modified_date:
---

正在规划做一下 Automation 脚本，这样平时工作可以快速做一些debug收集，而不是不停的翻找命令了，需要涉及到下列接口:

- cli命令格式
- linux root 进入后的命令以及debug命令
- netconf 命令及 notification 

这几天网上搜索了一下，,也简单尝试了一下命令，准备基于 paramiko/paramiko-expect 做些东西.
比较怀念以前用的 procomm 的 terminal ，在上面能快速开发做一些界面和脚本。因为本身是terminal平台，在上面运行脚本，调试很方便，随时介入.

对于网络设备的 Automation ,这一篇文章非常好，[A Tale of Five Python SSH LibrariesA Tale of Five Python SSH Libraries | The Elegant Network](https://elegantnetwork.github.io/posts/comparing-ssh/)

由此，才发现业界早已有NetDevOps的理念:
- [NetDevOps: When DevOps Comes To Networking - Opensense Labs](https://opensenselabs.com/blog/articles/netdevops)
- [​​What is NetDevOps? - Enterprise Networking Planet](https://www.enterprisenetworkingplanet.com/management/what-is-netdevops/)
- [What is NetDevOps? The top NetDevOps Tools for your Windows OS - Engineering Education (EngEd) Program - Section](https://www.section.io/engineering-education/what-is-netdevops-top-netdevops-tools-for-your-windows-operating-system/)

有比较配套的软件工具包，比如 [Nornir](https://pypi.org/project/nornir/) 
- [nornir 3.1.1 documentation](https://nornir.readthedocs.io/en/latest/)
- [【Nornir系列】NetDevOps自动化新贵：Nornir - 知乎](https://zhuanlan.zhihu.com/p/330734981)

还是希望从稍微基础点做起, summary:

- [pexpect](https://pexpect.readthedocs.io/en/stable/): 对于windows支持不是很给力。

    - 子模块 [popen_spawn](https://pexpect.readthedocs.io/en/stable/api/popen_spawn.html) 是给 windows spawn 用的。简单尝试了一下，进入linux后，发现buffer里有时候没有内容,再次read一下就有了。
    
    - ssh输入password 无法交互，用了 `ssh -t -t` 后勉强能用，但需要手工自己输入密码。

- [winexpect](https://github.com/geertj/winpexpect) 2011年后 没有更新

- [wexpect](https://github.com/raczben/wexpect) 情况好些，但是尝试了一下，还没有[popen_spawn](https://pexpect.readthedocs.io/en/stable/api/popen_spawn.html) 适用性好

- [paramiko](https://github.com/paramiko/paramiko) 基础功能强大

- [paramiko-expect](https://github.com/fgimian/paramiko-expect) 看着似乎很好用，下一步试一下.

- [asyncssh](https://github.com/ronf/asyncssh) [documentation](https://asyncssh.readthedocs.io/en/stable/#client-examples) asynch语法不懂，有时间再看

- [scrapli](https://pypi.org/project/scrapli/) [netmiko](https://pypi.org/project/netmiko/) 已经为一些路由设备做了定制，可以做参考


---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](./2022-05-12-note-xml-pexpect.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
