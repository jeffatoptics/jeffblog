---
title: Python rich库总结🎽
layout: post
category: coding
author: jeffatoptics
created: 2024-07-23 12:30
modified_date:
---

python rich 库作为终端控制工具，我非常喜欢。因此，做一个使用总结

1. inspect 函数

    inspect 方便直接在终端上直接读取参数的定义及架构，比 `print(help(xx))`要直观很多

    ```python
    teststr="this is a test string"
    inspect(teststr)
    inspect(teststr, methods=true)
    insepect(teststr, all=true)
    ```

1. print  print_json 函数

    rich print 风格更加清晰

1. 
---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](2024-07-21-running-at-sunday.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
