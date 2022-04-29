---
title: MPE inline code 很强大
layout: post
category: life
tags:
Author: 
- jeffatoptics
Created: 2022-04-29 Fri-17:50
---


没用过 [jupyter](https://pypi.org/project/jupyter/), 但看过它coding及输出结果直接在写文档的时候，直接交互生成。感觉很有意思。

采用MPE([markdown preview enhanced](https://shd101wyy.github.io/markdown-preview-enhanced/))后，发现它也支持python inline的方式。

前两天做过一次数测试据整理，在写文档的时候，直接coding读取测试数据，结果输出在文档里。
做完以后，
- 文档中直接用 import 语法 引用 python 程序，然后hide=true,感觉很清爽，

- <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>enter</kbd>运行后，直接输出结果在文档里, 直接允许功能很强大。

- markdown可以转化为html/pdf。

整个过程，只有在用vscode进行思考和调试，感觉很流畅。
按以前的方式，用excel，处理大约15M的测试数据，然后再绘图，比较卡。第一次需要类似处理时候，直接放弃了，画了两三个通道的数据作为代表就结束了。。

做个GIF图片记录一下


![](/assets/20220429/jeff-code-chunk.gif)



---
先做个测试，绝对路径引用
test absolute link [index](/index.md)
test relative link [index](../index.md)

---

---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](2022-04-29-mpe-inline-code.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
