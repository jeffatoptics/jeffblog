---
title: Zettelkasten note taking
layout: post
category: coding
mermaid: dark
author: 
- jeffatoptics
created: 2022-05-03 Tue 21:47
---

I am making this note in english, because the diagram i have plotted for a presentation was already in this language.


<div class='mermaid'>

flowchart LR;

FN(("fleet note"))
LN(("literature note"))
PN(("permanent note"))
PJN(("project note"))
RN(("reference note"))
ND[("Note DB")]
LD[("Literature DB")]

PN--->ND
LN--->LD
FN--->Recycle
PJN--->Recycle
FN---ReWriting-->PN
PJN--Manage-->FN & PN
PJN--Manage---->LN

RN-.-> PN & LN

style LN fill: red 
style PN fill: red
style FN fill: #0b0
style Recycle fill: yellow

</div>

As show in above figure, Zettelkasten note taking system looks quite complicated to me. Honestly, i do not fully understand how Luhmann manages his 90,000 cards with the above concepts. I am reading a book on that for inspiration, but it takes time.

However, one of his spirits is simple: making notes with your own words even with literate note, but not copy & paste.

I am now making my technical notes in with this idea.

My system is quite simple:

1. daily note: it collects my fleet ideas, and tips on different technical topics during my work

1. topic note: this address a topic which i have fully understood. it may be based on several daily notes

1. making limited tags in above notes to associate them. delete daily notes if its content is collected into the topic note.

My tool is mainly markdown extension MPE (https://shd101wyy.github.io/markdown-preview-enhanced/) in [vscode](https://code.visualstudio.com/). 
I also follow the note taking recipes from [FOAM/Github](https://github.com/foambubble/foam).

Below lists the major extensions i am using with vscode.

- [extension tool](../assets/file/2022-05-03-zettelkasten-extension.html)

Have a good note!



---

[⏮ home](../index.md) &nbsp; &nbsp; &nbsp; &nbsp; [🔀 category](../category.md) &nbsp; &nbsp; &nbsp; &nbsp; [◀️ prev](2022-05-03-make-emoji-colorful.md) &nbsp; &nbsp; &nbsp; &nbsp; [▶️ next]()

---
