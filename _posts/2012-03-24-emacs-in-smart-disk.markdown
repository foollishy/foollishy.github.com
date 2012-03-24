---
title: '在 U 盘上安个 Emacs'
layout: post
tags:
    - Emacs
---

用 Emacs 会上瘾的。虽然很少有机会用到，我还是想在 U 盘上安个 Emacs。

放"狗"搜了下，[安装过程][pigpog]很简单! 因为 for Windows 的 GNU Emacs 本身就是个"绿色"软件。大致过程如下:

- 在[官网][emacs]下载后解压至 U 盘;

- 在安装目录下的 /site-lisp/site-start.el 文件中中添加下面三行代码:

<pre class="lisp">
<code>
(defvar usb-drive-letter (substring data-directory 0 3))
(defvar usb-home-dir (concat usb-drive-letter "Home/"))
(setenv "HOME" usb-home-dir)
</code>
</pre>

- 在 U 盘根目录下新建一个名为 Home 的文件夹，然后把你的 .emacs 文件、.emacs.d 文件夹等都放进去。

- 搞定!

[pigpog]: http://pigpog.com/2007/10/22/portable-emacs-onna-stick/ "Portable Emacs-onna-Stick – USB Geekiness"
[emacs]: http://ftp.gnu.org/pub/gnu/emacs/windows/ "GNU Emacs"
