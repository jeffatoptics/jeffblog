---
title: 支持auto theme, katex以及mermaid
layout: post
category: coding
math: katex
mermaid: dark
author: 
- jeffatoptics
created: 2022-05-02 Mon 22:40
modified_date: 2022-05-04 
---

画了三四天时间把minima的 theme做了一些加强，东拼西凑的一些css /script ，效果还挺满意


$$
f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi
$$

<div class="mermaid">
graph LR
A(This is A)----->|this is demo text|B[(this is database<br><br> demo)]
C((This is C))--this is demo text--->B
D{This is D}--this is demo text--->B

    subgraph box
        A---C----D
        subgraph newbox
        C
        D
        end
    end
    subgraph box2
    B
    end
style B fill:#bbf,stroke:#000,stroke-width:4px,color:#f00,stroke-dasharray: 10 2
linkStyle 0 stroke:#f00,stroke-width:4px
</div>

![demo of jeff-minima](https://pic4.zhimg.com/80/v2-210dca306ac65bcf521a7c5e401589f8.gif)

---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](2022-04-29-image-in-recent-life.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next](2022-05-03-make-emoji-colorful.md)

---
