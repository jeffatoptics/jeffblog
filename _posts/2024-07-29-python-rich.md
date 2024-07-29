---
title: Python rich库总结
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

    rich print 风格更加清晰，考虑到与标准库print函数语法兼容,不会有额外的参数输入
    但能识别打印rich其他渲染体(renderable)

    ```python
    from rich import print
    from rich.console import Console
    from rich.text import Text
    console=Console()
    
    txt1=Text("this_is_str",style="blue on black")
    print(txt1)
    console.print("this_is_str", style="red on white")
    ```


1. console 类

    console.print

---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](2024-07-21-running-at-sunday.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
