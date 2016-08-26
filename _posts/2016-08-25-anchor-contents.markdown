---
layout:     post
title:      "Markdown 页内跳转"
subtitle:   "浅谈目录的构建"
date:       2016-08-25 21:42:00
author:     "Theo"
header-img: "img/post-bg/2016-08-25-anchor-contents.jpg"
catalog: true
tags:
    - Markdown
    - Sublime Text 3
---

上一篇博文里跟大家一起啃了啃 **Markdown** 的语法，其实已经可以满足写博文的基本需求了。Markdown 的本意是想让博主们专注内容的撰写而不是排版，但是如果硬要想做出更漂亮的排版，就需要偷偷学习一些**黑魔法**👊🎩。 

有时候一篇博文太长，我们会想建立一个**目录**，让小伙伴们能在宏观上把握全文的同时又可以自由的进行**页内跳转**，立即穿越到自己感兴趣的段子。今天就来聊一聊构建一个支持页内跳转的目录都有些什么奇技淫巧😏。

### 方法一：Markdown 和 HTML 混编

<span style="background-color:#2face6; color:#ffd109; padding:10px; border-radius:20px 0 20px 0;">废话不多说直接看代码：</span>

	* [主标题1](#1)
		* [副标题1.1](#1.1)
			* [次级副标题1.1.1](#1.1.1)
		* [副标题1.2](#one-point-two)

	<h1 id="1">主标题1</h1>
	文本内容。。。

	<h2 id="1.1">副标题1.1</h2>
	文本内容。。。

	<h3 id="1.1.1">次级副标题1.1.1</h3>
	文本内容。。。

	<h2 id="one-point-two">副标题1.2</h2>
	这是为了演示id也可以设置成英文字母

<span style="background-color:#2face6; color:#ffd109; padding:10px; border-radius:20px 0 20px 0;">效果：</span>

* [主标题1](#1)
	* [副标题1.1](#1.1)
		* [次级副标题1.1.1](#1.1.1)
	* [副标题1.2](#one-point-two)

<h1 id="1">主标题1</h1>
文本内容。。。

<h2 id="1.1">副标题1.1</h2>
文本内容。。。

<h3 id="1.1.1">次级副标题1.1.1</h3>
文本内容。。。

<h2 id="one-point-two">副标题1.2</h2>
这是为了演示id也可以设置成英文字母

### 方法二：Markdown 和 HTML 混编，利用 HTML 元素创建 "锚"

<span style="background-color:#2face6; color:#ffd109; padding:10px; border-radius:20px 0 20px 0;">其实第一种方法里已经有 "锚" 的概念了。看如下代码：</span>

```html
* [主标题1](#1)
	* [副标题1.1](#1.1)
		* [次级副标题1.1.1](#1.1.1)
	* [副标题1.2](#one-point-two)

<span id="1"></span>

# 主标题1
文本内容。。。

<span id="1.1"></span>

## 副标题1.1
文本内容。。。

<span id="1.1.1"></span>

### 次级副标题1.1.1
文本内容。。。

<span id="one-point-two"></span>

## 副标题1.2
这是为了演示id也可以设置成英文字母
```

<p style="border:3px solid #f95959; padding:10px; border-radius:20px;"><b>注意：</b><b>"锚"</b> 可以是 p 元素也可以是 a 元素也可以是 span 元素等等，<b>"锚"</b> 的下面建议空一行再写其他内容。因为效果和前面那个例子完全一样所以这里就不演示了。</p>

### 方法三：Markdown 原生支持的页内跳转?

<span style="background-color:#2face6; color:#ffd109; padding:10px; border-radius:20px 0 20px 0;">看代码：</span>

	* [Cat and dog](#cat-and-dog)
		* [Cat](#cat)
			* [A little cat](#a-little-cat)
		* [Dog](#dog)

	## Cat and dog

	一只单身狗和一只高冷猫的故事。。。

	### Cat

	有一天高冷猫遇见了单身狗。。。

	#### A little cat

	高冷猫生的很小巧但是脾气不是很好。。。

	### Dog

	可是，单身狗喜欢上了高冷猫。。。

<span style="background-color:#2face6; color:#ffd109; padding:10px; border-radius:20px 0 20px 0;">Theo 知道自己作文水平有限😂，客观先别急着笑，看下这段代码的效果：</span>

* [Cat and dog](#cat-and-dog)
	* [Cat](#cat)
		* [A little cat](#a-little-cat)
	* [Dog](#dog)

## Cat and dog

一只单身狗和一只高冷猫的故事。。。

### Cat

有一天高冷猫遇见了单身狗。。。

#### A little cat

高冷猫生的很小巧但是脾气不是很好。。。

### Dog

从此以后，单身狗喜欢上了高冷猫。。。

<p style="border:3px solid #f95959; padding:10px; border-radius:20px;"><b>注意：</b>Theo 编辑 <b>Markdown</b> 文本时使用的是 <b>Sublime Text 3</b>，测试页面显示效果时用的是一个叫 <b>OmniMarkupPreviewer</b> 的插件。在进行本地测试的时候 Theo 发现，如果单纯的用 <b>OmniMarkupPreviewer</b> 预览，这种写法的页内跳转是没有效果的。但是如果搭建本地 <b>Jekyll 服务器</b>，再用网页浏览器打开，跳转是有效的。另外，在 <b>Github</b> 上直接用这种 <b>Markdown</b> 语法书写，也是可以正常跳转的。<br>
因此结论就是你在浏览这段 <b>Demo</b> 时应该可以正常页内跳转，但是如果你书写并本地测试时发现无法正常跳转也不要感到稀奇，关于这个问题的解释可以引用<a target="_blank" href="https://www.zhihu.com/question/21907056">知乎</a>上的一个回答：</p>

> Markdown是没有一个所谓的规范的(作者都不支持这么做)，所以某些特性需要写作工具自己支持才可以。所以有可能A的markdown到B上就无法正确显示了。

---

OK，这些构造支持页内跳转目录的黑魔法你都学会了吗，快去活动活动手指，写一篇附带目录的长篇博文吧 O(∩_∩)O 哈哈~

###### 著作权声明

<span style="background-color:#f9e9a4; border-radius:5px; padding:5px;">博客内的文章如无特殊声明均为 Theo 原创，转载请保留原文链接，谢谢。<span>