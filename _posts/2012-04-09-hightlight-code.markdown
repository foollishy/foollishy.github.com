---
title: '从"代码高亮"说开去'
layout: post
tags:
    - learning
---

对于我这种英文水平一般的人而言，看原版书籍会有很多苦恼，其中之一就是随手翻开一页，看过去尽是蝌蚪文，不能将这些符号迅速转化成有意义的单词，得集中注意力才行。然而看中文书籍就不会有这个问题，大略扫几眼，就能知道大概了。这其中原理我不清楚，只知坚持阅读，水平高了，自然就能如读母语书籍一般。

除了英语，我对计算机技术也挺感兴趣，偶尔也会摆弄 XeTeX, Python, HTML 什么的(不过水平连菜鸟都算不上 XD)，知道很多文本编辑器或代码编辑器可以根据关键字来显示不的颜色和字体，增加代码的可读性，比如我上一篇 blog 里提到的一段:

<pre class="lisp">
<code>
(defvar usb-drive-letter (substring data-directory 0 3))
(defvar usb-home-dir (concat usb-drive-letter "Home/"))
(setenv "HOME" usb-home-dir)
</code>
</pre>

某一天我突发奇想，如果将英文书上的一些关键词用不同颜色的荧光笔做上记号，也来个"代码高亮"，效果该不会太差。拿手头上的 Word Power Made Easy 试了下，把新词和词根分别用不同颜色描出，效果真不错，有点上面提到的看中文书的感觉了。

![在英语书籍上用荧光笔做记号](../media/images/page_with_hightlight.jpg)

前两天看到李笑来[推荐](http://www.lixiaolai.com/archives/11595.html)了一款叫做"[单词圣手](https://chrome.google.com/webstore/detail/odhiddefamddbjhpaoagfkmgkkfhjnkd)"的 Chrome 浏览器扩展，眼前一亮:这不就是网页上的荧光笔嘛!

![单词圣手截图](../media/images/Smart_Word.png)

双击就可以将单词以不同的颜色显示；鼠标放到加亮的单词上会出现中文释义，同时还有发音；打开新网页，如果此页包含有以前标记过的单词，则会自动高亮显示。此扩展还支持将单词生成卡片、导出等功能，真是记忆单词的好帮手!

下载地址:https://chrome.google.com/webstore/detail/odhiddefamddbjhpaoagfkmgkkfhjnkd
