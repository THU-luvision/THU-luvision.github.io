---
layout: post
title: 怎样用 Atom+Markdown 写作
date: 2017-10-26 21:00:00 +0300
description: Markdown 是一种简单的语言，用它写作，就不用总想着用什么格式去修改。让写作回归写作的本质。 # Add post description (optional)
img: software.jpg # Add image post (optional)
tags: [Productivity] # add tag
---

Markdown 是一种简单的语言，用它写作，就不用总想着用什么格式去修改。让写作回归写作的本质。

先看三篇文章：
1. 用 Markdown 写作的好处见  [Markdown 写作浅谈](http://mp.weixin.qq.com/s/HsPZLl60vjbEKEbT2HHH7A)
2. Markdown 语法指南见  [Mastering Markdown · GitHub Guides](https://guides.github.com/features/mastering-markdown/)。
3. Atom 是开源的，支持很多 Markdown packages，可以扩展一些很赞的功能，Markdown 的预览，以及插入图片，看这篇文章就知道啦：[使用 Atom 打造无懈可击的 Markdown 编辑器](http://www.cnblogs.com/libin-1/p/6638165.html)。

你要是这三篇都看完，那Markdown的使用就基本没有问题了。

另外值得注意的是，GitHub Guides中没有提到 'color', 'css', 'html', or 'style'，因此用这些写的无法在 GitHub 上显示；下面的举例中，也会明确指出哪些适用于 GitHub，哪些不适用。

## emoji适用于（GitHub）

  如果是 GitHub写作，只要调用“：”就可以了。如果要在 Jekyll 中显示 emoji，还要注意 _config.yml中要这样[设置](https://help.github.com/articles/emoji-on-github-pages/)。

  在 Atom 里编辑 emoji，需要添加一个 package—[autocomplete-emojis](https://atom.io/packages/autocomplete-emojis)，输入“::”，就可以调用 Markdown emoji 了:smiley:

有哪些 emoji 可以用呢？来看看[小抄表](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

## 表格（适用于 GitHub）
  **Markdown 写法**

  ![table](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-20171026113646668.png?raw=true)

  **Markdown 呈现样式**

  |Softwa|Atom  |Jianshu|Weizhi|
  |------|------|------| ----|
  |Function|Edit|write |knowledge management|

## Highlight（适用于 GitHub）

![Highlight](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-20171026133106904.png?raw=true)

```diff
+ 加号代表highlight绿色
- 减号代表highlight红色
```

## 粘贴照片

为了快速粘贴剪切的照片，需在 Atom 设置中下载 [markdown-img-paste](https://atom.io/packages/markdown-img-paste)，并注册千牛云，按提示输入配置，其中域名只要用测试域名就可以了。

为什么不拷贝截图后直接粘贴，而要用千牛云呢，因为照片的路径无法在 Jekyll 页面上显示，只能在 GitHub 上显示。```Markdown-img-paste``` 默认粘贴的照片储存在 ```_post/assets``` 下，Jekyll直接找到 ```assets``` 上去找图片，是肯定找不到的。最好的解决方案还是用 ```Markdown-img-paste``` +千牛

![img-paste-setting](http://oysqcklir.bkt.clouddn.com/markdown-img-paste-20171103004943248.png)


## 字体(不适用于 GitHub)

  **Markdown 写法**

![font](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-2017102612053162.png?raw=true)

  **Markdown 呈现样式**

  1. <font face="黑体">我是黑体</font>
  1. <font face="微软雅黑">我是微软雅黑</font>
  1. <font color=#FF0000 face="宋体">我是红色宋体</font>
  1. <font color=gray size=5>我是灰色</font>

  另外颜色可以在这个网站查询[RGB颜色参考](http://tool.oschina.net/commons?type=3)

## 底色/背景色（不适用于 GitHub）

  **Markdown 写法**

![背景色](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-20171026125110889.png?raw=true)

  **Markdown 呈现样式**
  <table><tr><td bgcolor=#0e88e3>这里的背景色是#0e88e3</td></tr></table>

  配色参考 [Color Palettes Color Schemes](http://www.color-hex.com/color-palettes/)
