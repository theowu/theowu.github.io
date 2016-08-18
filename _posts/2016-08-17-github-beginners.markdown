---
layout:     post
title:      "献给小白的GitHub入门魔法书「译」"
subtitle:   "GitHub For Beginners: Don’t Get Scared, Get Started"
date:       2016-08-17 14:20:00
author:     "Theo"
header-img: "img/post-bg/2016-08-17-github-beginners.jpg"
header-mask: 0.3
catalog:    true
tags:
    - Git
    - GitHub
    - 译文
---

<!-- 由于GitHub项目空间有限，除了post-bg，所有图片全部host在OneDrive上 -->

> 这篇文章转载自 [readwrite网 CODE专栏 LAUREN ORSINI 发表的一篇文章](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/)。

原文作者是分成两篇**姊妹篇**写的，我一边翻译一边整合成一篇了。文章有些老(2013年写的😅)，之所以选中这篇文章，是因为：

- Theo在最近一篇博文里提到过Git，其实Theo也是前两天才学，所以写来自己复习。
- 原文写的确实很系统很好，连法国的博主都搬回去翻译过。
- 另外，如果你喜欢并已经会使用图形化操作界面的 **[桌面版GitHub](https://desktop.github.com)**，又不想和命令行或者 Terminal 打交道，你完全可以不学 **Git**，但是 **建议你最好还是了解一下背后的机理**。

**免责声明：**原文的内容会有改动，如果作者对此感到不爽可以<a target="_blank" href="http://theowu.tk/about/">联系我</a>进行修改或者删除，谢谢。

## 引语

> 这篇文章是献给小白们的，老鸟们笑笑就好。不喜勿拍。[你也可以戳我 👉 跳过废话，直接看正文](#main) 

> 相信小白们的世界里总会出现一个光怪陆离的物事那就是GitHub。至少Theo以前是这样的：<br>
有时候，下载一些开源软件，咦，怎么跑到这个不知所云的网站来了🤔。<br>
有时候，寻找一些下载网页视频的**黑魔法**，找了半天，在GitHub上找到解决方案了，感觉怎么这么 高! 大! 上! 😋。<br>
找一些插件、模板啦，动不动就有仙人指路👉GitHub。尼玛哥是小白耶! 要不要上来就拿这么专业的词汇砸我😡。。。<br>
哥开始学习苹果的Swift语言啦，矮油，怎么连Swift都托管在GitHub。。。好吧，哥可是精通搜索的 **"增长黑客"** ! 用百度谷歌一番发现怎么Git难道不是GitHub么😲😩。。。好麻烦啊，不管啦，反正差不多，反正下载东西很esay，你们做你们的大神，我做我的 伸! 手! 党! <br>找工作时招聘方要求精通Git版本管理系统，好吧凌乱的哥只想送他一句：你才Git呢，你们全家都GitHub了!!!

其实呢，**GitHub** 是一个很好用的**社交网站**! 对，你没听错，就像脸书啊人人之类的，只不过程序猿用的比较多，所以没有那种矫揉造作的某朋友圈😏。它同时是个附带版本管理系统的代码托管平台，所以成为了非常handy的合作生产工具。

施主，出来混，总有一天要学会宝刀怎么耍吧 。。。

<figure align="center">
	<img src="https://2xsexw.dm2301.livefilestore.com/y3mb7-b5x_EfKMFCH7Sk3sUiSrIWzMIn8DwgdCWR8NacJaH7xeAbiekwVKraXYEuEV7cDPRfjPmxQsBisGVvK2UcZ9LBvL2ZL-Usa8xctgohJWuFlJJLneGIQu1D42E6MUtLD6EmJzMMg1nIaDFzCYAAZR6PhHmhkvAH6L4aoGu5II?width=439&height=660&cropmode=none" width="219" height="330" style="border-radius:10px;">
</figure>


图片来源：[@新浪游戏](http://slide.games.sina.com.cn/c/slide_21_18723_33056.html#p=2)

<span id="main"></span>

## 目录

* [第一部分](#part01)
	* [01. GitHub寻寻觅觅](#01)
	* [02. 什么是Git? Git，GitHub 傻傻分不清](#02)
	* [03. Git的黑话](#03)
	* [04. Git特有的指令](#04)
	* [05. GitHub和Git的初始设置](#05)
	* [06. 创建线上Repo](#06)
	* [07. 创建本地Repo](#07)
* [第二部分](#part02)
	* [08. 联通本地Repo和GitHub线上Repo](#08)
	* [09. 汇总时间到!](#09)
	* [10. Git学习资源](#10)
* [著作权声明](#copyright)

<span id="part01"></span>

# 第一部分

2016年了，你逃不掉的：学不会 **GitHub** 就再也别出去撩妹了。

为什么? 因为它是一个颠覆我们工作方式的 **社交网络**。今天的 **GitHub** 已经从一个开发者的 **协同合作工作平台** 摇身一变成为了世界上最大的 **合作项目的集结地**。无论你是想下手和大家一起愉快地料理，还是继续做抓取人类知识结晶的伸手党，你都得去那里。

只要你注册一个账号，你就能像在谷歌和脸书上那样点赞社交。**GitHub** 创办之前，主流商业公司研究或者发现什么都是保密的。今天，当你逛到他们的 **GitHub** 主页，你可以免费下载，研究，学习他们托管在网上的所有东西，并以他们为材料去构建你想构建的任何东西。骚年，你还在等什么?

<span id="01"></span>

## 01. GitHub寻寻觅觅

令人尴尬的是，我撰写这篇博文是因为所有我读的"GitHub菜鸟教程"都让我看的一个头两个大。也许也是因为我编程基础差吧，其实大部分 **GitHub** 用户编程水准也没那么高😂。总之大部分教程都没把我这只笨鸟教会。

不过你有可能不知道，就算你不是一只程序猿，你也有一千零一条理由去用 **GitHub**。根据 **GitHub** 的教学视频，任何脑力工作者(其实就是搞电脑的)都可以从 **GitHub** 收益。

> 如果你之前放弃过学习 **GitHub**，这篇文章就是为你而写的。

有人说 **GitHub** 是个编码或者编译的开发工具，我想说你错了。**GitHub** 其实就是一个像Facebook和Flickr一样的 **社交网络**。你注册一个账号，上传分享一些项目，关注其他的用户，这样你们就互联了。很多人在 **GitHub** 上存放了很多程序和项目代码，其实你也可以存放一些文本文档或者其他格式的文档用来装B。

![](https://0xuf0w.dm2301.livefilestore.com/y3mxShykWcfrRvvV3C7Tvo3UDom6Th7Hty7vr6R8UkPuVoHvi5U__K1hbNV7XXEIMsjeP4zlxqZ1dGwXDVs1zRUc1ppF82dTNfGtvIOvUd2DSmz52dcqPhnery0eEI406ueJglvKp_LH-DH6aZix5xC3dFjzfekR4ugII_HFycmE34?width=1024&height=627&cropmode=none)
我的 **GitHub** 主页 ☝️

你的社交网络账号可能多的数不过来，但是我敢保证没有一个的[服务条款](https://help.github.com/articles/github-terms-of-service/)能好过 **GitHub** 的。如果你去瞅一眼条款的F项，你会发现**GitHub** 使出了吃奶的劲来保证你上传所有东西的所有权：

> "We claim no intellectual property rights over the material you provide to the Service. Your profile and materials uploaded remain yours."

更爽的是，就算你觉得代码看起来像天书，你也能使用 **GitHub**。你不需要任何教程就可以注册一个账号然后东踩踩西逛逛。但是我觉得最好还是从基础学起，就是说敲两行 **Git** 的命令。说到底 **GitHub** 其实是执行 **Git** 命令的最简单直白的 **图形化用户界面了**。  

<span id="02"></span>

## 02. 什么是Git? Git，GitHub 傻傻分不清

膜拜 **[Linux Torvalds](https://zh.wikipedia.org/wiki/林纳斯·托瓦兹)** 吧! 他是著名的软件开发者，**Linux操作系统**之父，就是这家伙写的 **Git** - 运行在 **GitHub** 核心的软件。**Git** 是一个版本控制软件，就是说它会在项目文件被修改的时候保证不覆盖这些文件。**Torvalds** 和他的核心开发成员使用 **Git** 去开发 **Linux** 的内核，**Git** 逐渐流行了起来。

为什么要玩 **Git** 这玩意? 想象一下你和你的同事同时在修改同一个网站的网页文件。你改你的，他改他的，能有什么问题? 假如你和他同时修改的是同一个网页文件，问题就来了。你们俩至少有一个人做出的修改会被另一个人干掉。

一个类似 **Git** 的版本控制应用可以避免以上情形的发生。你和你的同事可以同时上传对同一个文件的修改和校对，**Git** 会做两次备份。然后你们可以把文件的变动合并，这样不会丢失任何一方做出的修改。你甚至可以在任何时候把文件回滚到早前的版本，因为 **Git** 给每一个做出的修改都照了"快照"。

**Git** 的缺点就是年龄一大把了，我们只能像90年代的黑客一样在命令行(Mac上叫Terminal)里敲代码去调用它。这对于现代电脑用户来说有些坑。。。这就是为什么 **GitHub** 闪亮登场了。

![](https://1buf0w.dm2301.livefilestore.com/y3m06mkd3TuOhn50x0BtCX2BT3BwXvU6REpyjatwzs5dcUuYKYoZNtOEKL75kZbAQYcm3i1vWPBGi19DRq-kiE21xqNoF2DP4Vs96T6Rx7hKmZSCw1nrVNnFQPEImUj4pyfn_3l1iCedCCzCTDeEPVikmZiECMs35lkMWOUkGk6ovs?width=1024&height=659&cropmode=none)
我的 Macbook Pro 上的 Terminal 截屏 ☝️

**GitHub** 在两个层面使 **Git** 变得更加易用：

* 第一，如果你下载了 **[桌面版GitHub](https://desktop.github.com)**，你就拥有一个图形化的操作界面用来帮助你进行本地项目的版本控制。
* 第二，申请一个 **GitHub** 账号，你就可以将版本控制的项目传到网上备份，同时享受社交网路的功能。

你可以浏览其他 **GitHub** 用户上传的项目文件，甚至下载它们用于研究和学习。其他用户也可以浏览你公开的项目，帮你指出错误，提供技术支援。不管怎样，任何时候不会发生任何数据丢失，因为 **Git** 给每一个变更都照了"快照"。

虽然不用学 **Git** 就可以使用 **GitHub**，但是**使用**和**懂行**还是有区别的。在接触 **Git** 之前我就已经会用 **GitHub**，但是我其实并不明白工作机理。下面我们就来学学怎么在命令行工具里调用 **Git**。   

<span id="03"></span>

## 03. Git的黑话

江湖险恶，想跟 **Git** 打交道，得先学点 **Git** 的黑话：

**命令行 (Command Line)**:
一个用来输入 **Git** 命令的电脑程序，在Mac上叫 Terminal。Mac是编程神器，系统预装了 **Git**，但是版本有些陈旧，你可以[手动更新](#upgrade)。PC机上需要下载并安装 **Git**，命令行才会执行 **Git** 的相关指令。

**代码仓库 (Repository 简称 Repo)**: 一个存储你的项目的空间和目录。它可以是存储项目的本地文件夹，也可以是 **GitHub** 或者其他托管网站的存储空间。在这个空间里你可以保存代码，图片，文本文档。。。等等。

**版本控制 (Version Control)**:
这个就是 **Git** 被设计出来的目的了。如果你有一个 Microsoft Word 文档，要么你每次保存时都把老的版本覆盖掉，要么你要保存好多个文件。 有 **Git** 就不需要那样做， **Git** 会给每个变动来个"快照"(意思是它保存了单一文件的不同历史状态)。

**提交并备份/快照 (Commit)**:
这个词不知道该怎么译成中文，姑且意译了。**Commit** 功能就是 **Git** 的强大之处。当你 **Commit** 时，其实你是给你的Repo在一个时间点照了一个"快照"，就像一个随时可以回去的还原点。

**分支 (Branch)**: 
很多人怎么同时在同一个项目上修改呢? 一般而言，他们利用 **Git** 从主项目上造一个 **分支 (Branch)**，然后在自己的分支版本上修改。修改完成后，他们可以商量 **分支 (Branch)** 项目 和 **主 (Master)** 项目 的 **合并 (merge)** 事宜。

<span id="04"></span>

## 04. Git特有的指令

因为 **Git** 是为了 **Linux** 这样的庞大工程而诞生的，所以它有丰富的指令。但是你只要掌握几个以 `git` 关键字开头的命令就可以把它玩转了。

* `git init` ：初始化一个新的 **Git Repo**。你只有打开一个文件夹(这个文件夹就是你的本地Repo)，然后在命令行或者Terminal里敲这个命令之后才能运行其他指令。

* `git config` ：设置 (configure) 的缩写，这是你第一次部署 **Git** 时最有用的指令。 

* `git help` ：忘记指令咋写了? 在命令行敲这个来获取帮助。你也可以更具体些，例如输入 `git help init` 去查看 init 指令的作用和用法。

* `git status` ：查看 **Repo** 的状态。查看 **Repo** 里都有什么文件，哪些变动还没被"快照"(Commit)，还有你目前在 **Repo** 的哪一个 **Branch** 工作。 

* `git add` ：**注意，这个指令的意思不是把文件加到 Repo 目录下，而是让新文件进入到 Git 的关注范围**。运行完 add 指令后，**Git** 才知道要给这些文件照快照(这时 Git 还是不会自动存储变更的状态)。 

* `git commit` ：这是 **Git** 最核心的指令。你在 **Repo** 里做完任何修改后，在命令行输入这条指令，用来告诉 **Git**：好了，**Repo** 里的文件变更了，给我把变更后的状态照下来。常用的还有 `git commit -m "自己写点用来记录修改内容的文字"`。引号引起来的内容是你用来记录这次修改的，例如"增加新文件"啊，"修改内容"之类的。

* `git branch` ：和其他人合作，又想自己修改自己的。这个指令就可以让你创建一个新的分支，或者说新的快照时间线。你可以在最后输入新分支的名字，例如你想叫它"cats"，你就要在命令行里输入 `git branch cats`。 

* `git checkout` ：顾名思义，让你检查除去你手头正在工作的分支之外的另一个分支。**这是一个导航指令**。比如 `git branch master` 切换到主项目分支，`git branch cats` 切换到 cats 分支。

* `git merge` ：完成一个分支的修改后，你可以把你的修改合并到主分支，这样一来所有参与项目的开发者都能看到你修改的内容，例如 `git merge cats` 指令会把你在 cats 分支上所做的所有修改叠加到主分支上。

* `git push` ：把本地修改后的commits同步到 **GitHub** 线上。 

* `git pull` ：把 **GitHub** 上最新版本的 **Repo** 同步到本地以便于在此基础上进行修改。  

<span id="05"></span>

## 05. GitHub和Git的初始设置

首先，你要在 GitHub.com [注册一个账号](https://github.com)。这就像申请其他社交网站账号一样easy。记住你填的电子邮箱，后面会用到。

如果你注册完后什么都不做，**GitHub** 也能正常运作。但是如果你想在电脑**本地**工作，你就得[安装**Git**](https://git-scm.com) 了。

<span id="upgrade"></span>

> 这里再强调一下，如果你是 Mac 机，系统预装的 Git 版本可能有些陈旧。你可以在 Terminal 里输入 `git --version` 来检查 Git 的版本。写这篇博文时 Git 版本号已经更新到 2.9.3了，你可以直接在 [Git官网]((https://git-scm.com)) 下载最新版本安装。

安装完成后打开 Terminal，向 **Git** 介绍一下自己吧，输入以下命令：

	git config --global user.name "你的名字"

引号内输入你自己的名字，可以是真名，网名等，作为你的 **Git** 用户名。

然后，告诉 **Git** 你的 email。**这里要确保和申请 GitHub 账户时用一样的 email**：

	git config --global user.email "你的电子邮箱"

大功告成。(但是如果你想设置 **Git** 让它不要每次都让你登录你的 **GitHub** 账号，你可以在[这里](https://help.github.com/articles/set-up-git/)找到更详尽的操作步骤。)

<span id="06"></span>

## 06. 创建线上Repo

现在你已经全部部署好了，是时候为你的第一个项目创建一个 **Repo** 了 - 一个保存所有项目文件和所有版本状态快照的目录或者空间。

在 GitHub.com 上登录你的账户，右上角你的头像左边的加号上点一下，选择 "New Repository"，然后你会看到如下界面：

![](https://1ruf0w.dm2301.livefilestore.com/y3mZKJJgyOAXLPK2lVQeChS568m2xqTBkpAUq__Nm6qYZwG6fp5ibqcD8KQo9LkstNb5OZ9kozlIU44ctqeZhCOtVGlizGhrypxn0l9pWnqyg0YaYnU8ItMjTzL9w0OzOyZ9v2IGd6VDFbTz0_K2E2O-TyuG7oQUJZ_lIT99Ueb718?width=1024&height=731&cropmode=none)

给你的 **Repo** 一个简短易记的名字(好像不支持中文)，然后勾选 Public 开放访问权限，让别人笑去吧，学习 **GitHub** 有什么好藏着掖着哒?

勾选或者不勾选 "Initialize this repository with a README" 看你心情。README 文件其实就是你的项目描述文件。

最后猛戳那个绿油油的巨大按钮。你的线上项目 **Repo** 就这么创建好啦!   

<span id="07"></span>

## 07. 创建本地Repo

我们刚刚为你的项目在网上建立了一个存储仓库，但是你不用在线上工作。你的大部分工作将在本地完成。所以我们要将这个线上 **Repo** 映射到一个本地的文件目录。

这部分涉及的命令行代码比较多，所以我经常在读其他教程贴关于这部分的内容时被搞得蒙圈。所以我们一步一步慢慢来。

首先在 Terminal 输入：

	mkdir ~/MyProject

`mkdir` 是 "make directory" (创建的文件目录) 的简写。她不是一个	**Git**	特有的命令，它是一条在我们能看到电脑图形界面之前就可以运行的导航指令。`~/` 的意思是电脑里用户文件夹的根目录，比如我的用户文件夹叫theowu，那么 `~/` 就指代的是theowu文件目录。如果你还是不明白，你可以在**文件浏览器**的**地址栏**输入 `~/` 看看它在你的电脑里具体在哪里 (**注意**，是**文件浏览器**，不是**网页浏览器**。PC上的文件浏览器很简单，随便打开一个文件夹的界面就可以了)。如果我没记错的话，Mac 用户要在 Finder 菜单栏选择 Go to 然后 Go to folder，然后输入 `~/`。其实你也可以在**网页浏览器**的**地址栏**里输入 `~/` 来查看目录具体在哪，目录下都有什么文件，只是在 Mac 上 Safari 浏览器似乎有些问题，你换成 Chrome 试试。

另外，注意我创建的文件目录名字叫 MyProject，和前面在 **GitHub** 上创建的 **Repo** 的名称一致。你也要养成好习惯，两次使用相同的名称。

现在终于可以用一个 **Git** 命令了，在命令行下一行键入：

	git init

**Git** 命令全都是以 **Git** 关键字开头的，用以和其他命令区分。`init` 的意思是 "initialize" (初始化)，它告诉电脑把当前所在文件目录视为 **Git** 的本地 **Repo**。

以上命令执行完后你的电脑就意识到该文件目录已经部署好 **Git** 了，你就可以下达其他 **Git** 相关的指令了。现在你在线上和线下都有用来存储项目文件的 **Repo** 了。下面宝宝就来学着给本地和 **GitHub** 上的  **Repo** 进行第一次 **Commit**。更多优质的 **GitHub** 学习资源在向你招手👏。

<span id="part02"></span>

# 第二部分

如果你成功的搞定了上面的步骤，恭喜你👊，我看你定是骨骼惊奇🤔，将来必成一代棕狮🦁! 我们现在就往项目目录里塞点东西，然后弱弱地  **Commit** 一下😏。对了忘记说了，前面创建了 MyProject 目录，但是没有进入该目录，为保证在该目录下操作，再在命令行输入 `cd ~/MyProject`。`cd` 是进入的意思。现在确保你的命令行大概是这个样子：

![](https://zhuf0w.dm2301.livefilestore.com/y3mqAsbN8EzURSDRaKuEDASY6iUUnCXhaT7gcZeVVTV_H78vCDra2bKnp99KRpcBtsOErZvJcXlLfHJPGfRau2ldwSHCccu3j6HI3MByPYKN8Bgiq0vrb30CLeS_K9xUbuK2D2OCZOnAo7lfQJDn8Nth1yQHM4Ws8r5OJn6OM_AcdA?width=1024&height=423&cropmode=none)

下一行输入：

	touch Readme.txt

这不是一个 **Git** 特有的命令，这是另一个标准导航指令。`touch` 的其实是 "create" 即创建的意思，后面跟的是你要创建的东西的名字。如果运行完该指令后你用文件浏览器或者 Finder 浏览到 MyProject 目录下你会发现里面多了一个空的 Readme.txt 文件。如果你调皮又贪玩，你也可以创建 Readme.doc 或者 Kiwi.gif 等等。

你能清晰地看见新增的 Readme.txt 文件， **Git** 可不一定。让我们测试一下。下一行输入：

	git status

然后你大概会得到这样的回复：

![](https://zxuf0w.dm2301.livefilestore.com/y3mD8_ZbY0gURaagX0E3pgxA8DLNlTaNemaqYJ7ovhrlIZLmXmyJ9LnUEOw-fHngs7cIUUUXo9TONErdUg7KTJ1KNGinMwLdpQ4xHrtyvArcqvYKomafdGsKYIrnfeyrVsp9UNsmnOAAUFIxK3UXbtg7Dk5VGpURGsVEd4Ljejb9eM?width=1024&height=530&cropmode=none)

	On branch master

	Initial commit

	Untracked files:
  		(use "git add <file>..." to include in what will be committed)

		Readme.txt

神马情况?!<br>
首先，第一句是说，你现在处于主分支(master branch)，显然你在主分支，因为你从来没创建过其他分支，而且你是一个人在工作，也没有别人创建其他分支。<br>
其次，Readme.txt 文件被列为 "untracked file"，英语不好的童鞋蛋疼了，其实是**未被追踪的文件**的意思，也就是说 **Git** 忽略的文件。要让 **Git** 关注这个文件的变动，在命令行键入：

    git add Readme.txt

好啦，现在 **Git** 知道要时刻关注这个文件是否变动了。是时候给整个工程项目来张美照了，或者说小小的 **Commit** 一下，在命令行键入：

	git commit -m "Add Readme.txt"

![](https://0buf0w.dm2301.livefilestore.com/y3mAGxlYo6WP615wNmcOAp1gSKKFEAwakb4b9UID7EVDLbMgLSY076VKq4SuCmBPdegGd88NthrJmvfMUJ5VryiPTOpdvToqnntqfOL8Nbfh_qtRxKpb1VM--tTy3-14owWQch0EkQ_SKJ8DWEtXfapSe8ApalCAxSG-GX_165UBpA?width=1024&height=530&cropmode=none)

`-m` 意思是 message (消息)，什么消息呢，就是刚才项目文件变动的描述。注意描述是用现代时写的，不是过去时，因为你可能随时想回滚文件版本，所以养成好习惯，用现在时描述一个 **Commit**。

刚才我们在本地做出了一些变动，是时候把我们的第一个 **Commit** 也同步到你的 **GitHub** 上了。

等等，你可能会想，我们还没有把线上 **Repo** 和本地 **Repo** 联通起来呢。Bingo! 的确如此，那么下面我们就来建立这样一个联接。

<span id="08"></span>

## 08. 联通本地Repo和GitHub线上Repo

同时拥有本地和远程 **Repo** 是美妙的🎊🎉。**你可以在本地一心一意地敲敲打打修修补补，不用管朋友圈里的炫耀谎言谣言或者其他怪相或者烂事**，等你完工后只要退送到 **GitHub** 就可以骄傲滴让你的小伙伴们看到你都捣鼓了啥子出来😋。

这样做也方便多个小伙伴在同一个项目上贡献自己的力量。小伙伴们可以在自己的电脑上各行其事，完工后把自己的成果推送到 **GitHub** 上。So，小伙伴们，让我们开黑吧!

首先，我们得告诉 **Git** 在线上某处存在这样一个远程 **Repo**。

假设我们在 **GitHub** 上有一个叫 "MyProject" 的 **Repo**，位于 http://github.com/`用户名`/`项目名`.git。当然啦，`用户名` 得换成你的 **GitHub** 用户名，`项目名` 得换成你给你第一个 **GitHub Repo** 起的名字。实际上，你可以登录你的 **GitHub** 主页，在项目子页面里找到该项目的网络地址。

一切就绪后在命令行键入：

	git remote add origin http://github.com/用户名/项目名.git

翻译过来就是：**git 远程 添加 源 http://github.com/`用户名`/`项目名`.git**。不用Theo解释，聪明如你应该会懂吧。

**Git** 现在知道这个线上 **Repo** 的存在了，那就是你本地做出的修改要同步过去的地方。命令行键入以下命令确认一下：

	git remote -v

![](https://0ruf0w.dm2301.livefilestore.com/y3mnw9GrgiX3_B0-sYXiYtGYj7v5M43Fy5ACvBoxYRHOD5M9wQv0vZW767QUqS62oiPQfQ-BvjrnRdQK8OEmnwBWMxTon3TnyUwAa9zqrVKxk2_ITFeXTP-aBnULLoEQLeUOwV90DSHDfi6eo3XhvVk67Aye-4bBavJ4rsQXvLPtoA?width=1024&height=530&cropmode=none)

运行完命令后，控制台给你返回了一个列表，里面包含的是你的本地 **Repo** 所识别的所有远程源。如果你前面一直跟着我的教程做的，那么这里应该只有一个源。这个源被列举了两次，第一次意思是说你可以从这个源上 **fetch (抓取)** 信息，第二条意思是说你可以向这个源 **push (推送)** 信息。

现在我们想做的就是上传或者说 **push (推送)** 本地文件的变动到 **GitHub** 的远程 **Repo**。那么简单了，在命令行键入：

	git push origin master

![](https://2huf0w.dm2301.livefilestore.com/y3mJATP_AqCvb6xpATxYhOCVs-tSHamZYU5KNu06bVSn29VrudtTtNvQ1tGGOYQS2xnNai_8hoBbht6e95YFcA8Uuh56LL3R7BtxxNIYEwy8-D1jpKjq8MisXNXWIgoOzGxva4yVKekxTwntmz6VaSVXnK0zrEBD08Cd8ZPFC-7Slo?width=1024&height=241&cropmode=none)

这句命令的意思把所有变动以及快照统统 **push (推送)** 到刚才设定的那个源的主分支。登录你的 **GitHub**，你会看到 **GitHub** 已经在记录你今天的 **Commit** 次数了。如果你进到项目目录下，你会发现多了一个和本地项目目录下一模一样 Readme.txt 文件。

<span id="09"></span>

## 09. 汇总时间到!

恭喜你! 🎉🎊 你现在已经正式从小白晋升成一个把 **Git** 舞得虎虎生风的叫兽了。你现在会创建 **Repo** 了，也会 **Commit** 了。网上的很多教程到这里就要结束了。

但是你也许会觉得："我读书少，表骗我😒"，或者内心有一万只**草泥马**在奔腾。你确定这样就可以自己动手丰衣足食了吗，至少我是不行的。

<figure>
    <img src="https://2xuf0w.dm2301.livefilestore.com/y3pdhgorMi2PJRiD7nZDiR4EctAqOMofpvPCZZrpRcfIvRaGkEkWEHVt-Y2lb5LIoJAQkPUVHSpi9WfpEgn-qT-hs2VK_kOLIyv7SsXD7aaeK-CzOBXYSRhtQ6kl6H7wO0x5jHeNqzxGOYgjheE1wIFaw/alpaca.gif" width="240" height="145">
    <img src="https://0htiow.dm2301.livefilestore.com/y3mJkndXMKaPgnk4BeTT_G8RPFC4tZeiP9dPtkkATgIhvVpW77LcKWgqC4Gl6sq-GLV5ccgVcgSIfk8ztDBnRrG7yt3rlXh88E50zYCDh_h0kUFL-jxNSbtGDI2t9jdeLY0Xr202vIqi66obBAsZW3Mb2GpkdUZu4gp-9ZuGvBuQCg?width=500&height=273&cropmode=none" width="240" height="145">
    <img src="https://0xtiow.dm2301.livefilestore.com/y3mD0RoZ63KZLeAWvdw7V67AcIriIZ20rpM9M2V1Wo-qkxXXZJUeJzIrc4wXkUvwQBMpSOYedR-8jRJx7sw8ed3WQMG7B5KXXTC8bc-QnXOhkkwrVeZbistk8Yo8_O1uS4nycyzkPio6vX24HLF8qJSnzFJzSx9CeFzMLnKP8sRHCc?width=640&height=386&cropmode=none" width="240" height="145">
</figure>

图片来源：[@今日头条-爱她就给她一场草泥马婚礼](http://toutiao.com/i6230911066537198081/)

为了真正的玩转 **Git**，让我们用所学的所有技巧来模拟一次完整的 **Git** 工作流程。

假设你现在是某鹅厂的网页设计师，你正在和团队里其他一些小伙伴们一起开发一个新的鹅厂子站叫草泥马网。

当你的上级告诉你该网站的初代设计太low了你将参加重新设计草泥马网的网页时，你觉得作为一个没有程序猿🙈背景的UX设计狮🦁马上要开始装B了真特么是既紧张又鸡冻🐔。但是你的Boss向你保证说谁都能快速学会用 **Git**。

于是你上网找了一些图片资源，大刀阔斧地PS成了一系列滑稽又可笑的网站吉祥物的图片😂，你把这些图片保存在了本地一个叫alpaca的文件夹里。现在你得把它加入到项目文件目录里了。

打开 Terminal，更改文件目录直到你进入到这个alpaca文件夹里面，因为你的图片都存在那里。比如这样：

	cd ~/alpaca

然后初始化 **Git** 以便能在该文件目录下使用 **Git** 命令。在命令行键入：

	git init

现在这个文件夹已经是一个 **Git Repo** 了。检查一下你是否确实处于存储你的图片的那个文件夹，命令行键入：

	git status

为了模拟真实情景，Theo早前在alpaca文件夹里丢了三个文件：`一群草泥马.jpeg`，`草泥马.jpeg`，和 `蓝色草泥马.jpeg`，所以 **Git** 给我的回复是这样的：

	On branch master

	Initial commit

	Untracked files:
  		(use "git add <file>..." to include in what will be committed)

			一群草泥马.jpeg
			草泥马.jpeg
			蓝色草泥马.jpeg

发现了没，你P的图全在那里了(假设这三个文件是你的P图成果😂)。接下来用 add 命令告诉 **Git** 去关注它们，键入命令：

	git add 草泥马.jpeg

然后用 commit 命令给你的 **Repo** 照张"快照"并注解一下：

	git commit -m "Add 草泥马.jpeg"

现在你的控制台应该是类似这样子了👇：

![](https://1btiow.dm2301.livefilestore.com/y3mQAW93Klu6q1qUWhrPEyPM5sj8D61MFpQW5fLGnwOk09dAeVuJgy_f8M1oM8U6OWzTEVK-VW2Y1kzrgqihI0sEfYg2Ms_1KiezyG91xiSfk7w_VPoLZCL6bHQMl9_SXtt-u_co6yD3eHxY9OtVIo6_8-33tEJAC5YGHy5RwVuTEg?width=1024&height=659&cropmode=none)

其实一个一个 add 太麻烦，你也可以用一个 \* 通配符一次性把目录下所有文件添加到 **Git** 的关注范围内：

	git add *

养成好习惯，每次 add 之后都要 commit 并注解：

	git commit -m "Add all files"

太棒啦! 但是团队里的其他小伙伴在各自的 **Repo** 埋头苦干根本看不到你的杰作，因为主项目文件都托管在你们公司的 **GitHub** 账户 (用户名: gooseWebDesign) 上名叫 "alpaca"的 **Repo** 里。

你还没有连接到这个 **GitHub Repo**，所以电脑连它是什么鬼都不知道，告诉你的本地 **Repo** 这个线上 **Repo** 的存在吧：

	git remote add origin https://github.com/gooseWebDesign/alpaca.git

保险起见，再用以下命令检查一下：

	git remote -v

最后，期待已久的时刻终于来临了。把你P出来的滑稽又可笑的网站吉祥物图片连同刚才做过的commit一起全部推送到公司的工程项目里吧：

	git push

嗒啦! 🎉🎊 有这些便捷的功能，**Git** 和 **GitHub** 显然不仅仅是程(zhòng)序(yīn)猿(zài)们(zhè)的屠龙宝刀。

<span id="10"></span>

## 10. Git学习资源

我知道，**Git** 是块难啃的骨头。我已经尽力把教程写的让我这种天然呆都能看懂，但我知道每个人有每个人的学习方式。还是没能搞明白的童鞋，以下是其他一些学习 **Git** 和 **GitHub** 的资源：

| 标题        	    | 注解          	|
| ----------------- | ------------- |
| [Is Git the Same Thing as Github!?](https://jahya.net/blog/git-vs-github/) | 这篇文章很好的解释了 **Git** 和 **GitHub** 的区别。 |
| [多用Git少交税](http://1ke.co/course/342) | 一篇用包包子打比方解释 **Git** 运作机理的博文。 |
| [Pro Git](https://git-scm.com/book/en/v2) | 一整本详尽开源的 **Git** 学习用书， **Git** 官方推荐。 |
| [Try Git](https://www.codeschool.com/courses/try-git) | **CodeSchool** 和 **GitHub** 联合制作了这个快速入门教程。如果你想多学点操作基础，这个教程会很有帮助。如果你很壕，你可以在 **CodeSchool** 上撒点银子，你将学会所有关于 **Git** 的知识。 |
| [GitHub Guides](https://www.youtube.com/c/githubguides) | 如果你喜欢看视频学习，你可以去逛逛这个 **GitHub** 的官方油管频道。 |
| [Git Reference](http://gitref.org) | 学会了基础但是老是忘记指令怎么写? 来看看这个字典式参考站点。 |
| [Git – the simple guide](http://rogerdudler.github.io/git-guide/) | 一个机智简短的教程，但是对于小白而言会不会节奏过快了。如果你想快速复习一遍，这篇教程是不错的选择。 |

<span id="copyright"></span>

### 著作权声明

* 本文译自 [GitHub For Beginners: Don’t Get Scared, Get Started](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/)<br>
以及其姊妹篇 [GitHub For Beginners: Commit, Push And Go](http://readwrite.com/2013/10/02/github-for-beginners-part-2/)

* 还有法国友人译成了法语版，感兴趣的可以读读 [GitHub Pour les Nuls: Pas de Panique, Lancez-Vous!](http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/)<br>
法语版第二部分 [GitHub pour les Débutants: Consignez, Poussez et Foncez!](http://christopheducamp.com/2013/12/16/gitHub-pour-nuls-partie-2/)

* 本文中文版本由 [@吴思元](https://www.zhihu.com/people/theowu) 独家翻译，首次发布于[Theo's Blog](http://theowu.tk)，转载请保留原文链接，谢谢。
