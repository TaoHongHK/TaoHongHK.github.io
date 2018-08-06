---
layout: post
title: The Summer Life
date: 2018-08-05 13:32:20 +0300
description: First Blog. # Add post description (optional)
img: post-2.jpg # Add image post (optional)
tags: [Blog, Meditation]
author: hongtao # Add name author (optional)
---

# **暑假的学习**

标签 : 学习篇

---

> [TOC]

## **自己的博客**

### 1.为什么创建自己的博客

开通博客无非是~~为了装逼~~为自己的学习或生活做一个记录，我也是想记录一下自己的大学生活，毕竟谁也不 想混个四年是吧，我的文笔差劲的很，如何有其他的人看我的博客，应该会很难受吧，哈哈，那就没办法了

---

### 2.如何创建一个自己的博客

>* 首先我利用github.io创建了一个最简的博客，选用的是官方推送的几个主题之一，网上教程贼多
>* 如果你只想要一个最简单能够发布的博客的话，那么以上步骤就足以满足你了，如果你像我这样想要骚气一点的话，你可以继续往下看
>* 首先去下载ruby并安装，然后再去下载Devikit并安装，(由于网络问题，不翻墙的话是无法下载官方文件的，但是国内的软件网站有很多的下载途径)，下载完成后进入ruby，输入 `$ gem install jekyll` 安装jekyll，输入`$ jekyll -vv`查看是否安装完成
>* jekyll tree的结构一般如下
```
├── _config.yml
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   ├── post.html
|   └── page.html
├── _posts
|   └── 2018-01-11-welcome-to-jekyll.md
├── _sass
|   ├── _base.scss
|   ├── _layout.scss
|   └── _syntax-highlighting.scss
├── about.md
├── css
|   └── main.scss
├── feed.xml
└── index.html
```
>* 安装完成后，你就可以去[选择jekyll模板了](http://jekyllthemes.org/)
>* 选择好后，将你所看中的模板下载下来，将文件复制到你的github.io库的本地库文件中（需要提前clone到本地），改变其中的config文件，将所需的配置改为你自己的，就大功告成啦！

---

### 3.如何去书写自己的博客

由于githu.io支持的是markdown语法书写，所以用github做博客的朋友要花一点时间去学习一下，其实markdown语言是十分简单的，学起来非常快。

什么是markdown:
:    Markdown 是一种轻量级的「标记语言」，它的优点很多，目前也被越来越多的写作爱好者，撰稿者广泛使用。看到这里请不要被「标记」、「语言」所迷惑，Markdown 的语法十分简单。常用的标记符号也不超过十个，这种相对于更为复杂的 HTML 标记语言来说，Markdown 可谓是十分轻量的，学习成本也不需要太多，且一旦熟悉这种语法规则，会有一劳永逸的效果。

如何使用markdown:
:    看看就会了[markdown手册](https://www.zybuluo.com/mdeditor?url=https://www.zybuluo.com/static/editor/md-help.markdown)


## **搞一下Java**





[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
