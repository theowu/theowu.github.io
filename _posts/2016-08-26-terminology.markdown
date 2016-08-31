---
layout:     post
title:      "术语笔记"
subtitle:   "梳理一下各种让人摸不着头的Terminology"
date:       2016-08-26 14:04:00
author:     "Theo"
header-img: "img/post-bg/2016-08-26-terminology.jpg"
catalog: true
tags:
    - 前端
    - 移动开发 Mobile
    - 网络开发 Web
    - 术语 Terminology
    - iOS
    - 软件工程方法学
---

这几天学了很多专有名词，学的 Theo 都快蒙圈了。今天就来把这些Terminology来个大汇总吧✅👊!

#### 小目录
* [软件工程方法学](#methodology)
* [iOS 开发](#iOS)
* [Web 前端开发](#front)
* [Web 后端开发](#end)
* [数据库](#dataBase)
* [小窍门](#tip)

<h3 id="methodology">软件工程方法学</h3>

<!-- Iterative and incremental development -->
<h5><span style="background-color:#f98178; color:white; padding: 10px; border-radius:10px 10px 0 0;">Iterative and incremental development</span></h5>

**迭代增量式开发**或迭代进化式开发，是一种与传统的**[瀑布式开发](https://zh.wikipedia.org/wiki/瀑布模型)**相反的软件开发过程，它弥补了传统开发方式中的一些弱点，具有更高的成功率和生产率。

在**迭代式开发方法**中，整个开发工作被组织为一系列的短小的、固定长度（如3周）的小项目，被称为一系列的**迭代**。每一次迭代都包括了**需求分析、设计、实现与测试**。采用这种方法，**开发工作可以在需求被完整地确定之前启动**，并在一次迭代中完成系统的一部分功能或业务逻辑的开发工作。再通过客户的**反馈**来细化需求，并开始新一轮的迭代。

<span style="border:2px solid #f98178; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[迭代增量式开发](https://zh.wikipedia.org/wiki/迭代式开发)
<br><br>

<!-- Agile software development [EN] / méthode agile [FR] -->
<h5><span style="background-color:#f98178; color:white; padding: 10px; border-radius:10px 10px 0 0;">Agile software development [EN] / méthode agile [FR]</span></h5>

**敏捷软件开发（Agile software development）**是一种从1990年开始逐渐引起广泛关注的 **一些新型软件开发方法**，是一种应对快速变化的需求的一种软件开发能力。它们的具体名称、理念、过程、术语都不尽相同，相对于「非敏捷」，**更强调程序员团队与业务专家之间的紧密协作、面对面的沟通（被认为比书面的文档更有效）、频繁交付新的软件版本、紧凑而自我组织型的团队、能够很好地适应需求变化的代码编写和团队组织方法，也更注重软件开发过程中人的作用**。

* **敏捷方法** 有时候被误认为是无计划性和纪律性的方法，实际上更确切的说法是**敏捷方法强调适应性而非预见性**。

* 相比 **迭代式开发** 两者都强调在较短的开发周期提交软件，敏捷方法的周期可能更短，并且更加强调队伍中的高度协作。

* **敏捷方法** 和 **瀑布式开发** 没有很多的共同点，**瀑布模型** 是最典型的**预见性的方法**，严格遵循预先计划的需求、分析、设计、编码、测试的步骤顺序进行。步骤成果作为衡量进度的方法，例如需求规格，设计文档，测试计划和代码审阅等等。

<span style="border:2px solid #f98178; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[敏捷软件开发](https://zh.wikipedia.org/wiki/敏捷软件开发#.E5.AF.B9.E6.AF.94.E7.80.91.E5.B8.83.E5.BC.8F.E5.BC.80.E5.8F.91)
<br><br>

<!-- Scrum -->
<h5><span style="background-color:#01d453; color:white; padding: 10px; border-radius:10px 10px 0 0;">Scrum</span></h5>

**Scrum** 是一种 **用于管理软件产品开发进度的**，**迭代增量式** **敏捷软件**开发过程的框架，它规定了软件开发过程中的一系列做法和角色分配。**Scrum** 在英语是橄榄球运动中的**争球**的意思。虽然 **Scrum** 方法是为管理软件开发项目而被发明的，它同样可以用于运行软件维护团队，或者作为营销项目管理方法。**Scrum** 之间的合作称为 ***Scrum of Scrums***。

**Scrum** 中的主要角色包括：

* **Scrum Master**：为 **Scrum 过程** 负责的人，确保 **scrum** 的正确使用，帮助团队扫除实施 **Scrum** 的障碍并使得 **Scrum** 的收益最大化。
* **产品负责人**：确定产品的方向和愿景，定义产品发布的内容、优先级及交付时间，为产品投資回报率负责；
* **开发团队**：一个自我管理的跨职能的小团队，人数5-9人，团队拥有交付可用软件需要的各种技能。

按照对开发过程的参与情况，这些角色被分为两组，即 **猪组** 和 **鸡组**。这个分组方法的由来是一个关于猪和鸡合伙开餐馆的笑话：

> 一天，一头猪和一只鸡在路上散步。鸡对猪说：“嗨，我们合伙开一家餐馆怎么样？”猪回头看了一下鸡说：“好主意，那你准备给餐馆起什么名字呢？”鸡想了想说：“叫‘火腿和鸡蛋’怎么样？”“那可不行”，猪说：“我把自己全搭进去了，而你只是参与而已。”

**猪组成员**：包括Scrum主管，产品负责人，开发团队等承担实际工作的人员。

**鸡组成员**：包括用户，利益相关者（客户，提供商，经理(为产品开发团体搭建环境的人)。

**Scrum** 工作流：

* **Planning**：每个冲刺开始时的会议，用来确认这次冲刺阶段的大致工作内容，具体化产品订单，给开发团队分配任务。
* **Daily Scrum**：在冲刺中每天都会举行的项目状况会议。
* **Review and retrospective**：冲刺结束阶段举行的总结和展望性质的会议。
* **Extensions**：一些其他诸如 Backlog refinement (订单精细化)，Scrum of Scrums (和其他 Scrum 团队的沟通及合作) 等等活动。

一些 **Scrum** 术语：

* **Sprint**：冲刺或者迭代，是 **Scrum** 开发过程中的最小时间周期，通常在2周到1个月之间，开发团队会在此期间内完成所承诺的一组订单项的开发。
* **Spike**：一个概念研发和简单模型创建的时限。
* **Product Backlog**：产品订单，括所有所需特性的粗略的描述。
* **Sprint Backlog**：冲刺订单，是大大细化了的文档，包含团队如何实现下一个冲刺的需求的信息。

<span style="border:2px solid #01d453; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[Scrum](https://zh.wikipedia.org/wiki/Scrum)
<br><br>

<!-- Extreme programming [EN] / eXtreme Programming [FR] -->
<h5><span style="background-color:#01d453; color:white; padding: 10px; border-radius:10px 10px 0 0;">Extreme programming [EN] / eXtreme Programming [FR]</span></h5>

**极限编程** (缩写为XP），是一种 **软件工程方法学**，是 **敏捷软件开发** 中最富有成效的几种方法学之一。该方法的推崇者认为该方法把传统的软件工程中最有益的做法发挥到了极致，因此把该方法命名为 **极限编程** 。

如同其他 **敏捷方法学**，**极限编程** 和传统方法学的本质不同在于它更强调可适应性而不是可预测性。**极限编程** 的支持者认为软件需求的不断变化是很自然的现象，是软件项目开发中不可避免的、应该被欣然接受的现象；他们相信，和传统的在项目起始阶段定义好所有需求再费尽心思的控制变化的方法相比，有能力在项目周期的任何阶段去适应变化，将是更加现实更加有效的方法。因此 **极限编程** 推崇短周期的小幅版本更新，双人合作编程，高强度代码重读，高强度测试，避免编写新功能(除非真正需要)，扁平的管理架构，简单和简洁的代码，用户和程序员之间的频繁交流与沟通。

<span style="border:2px solid #01d453; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[极限编程](https://zh.wikipedia.org/wiki/极限编程)
<br><br>

<!-- --------------------------------------- -->

<h3 id="iOS">iOS 开发</h3>

<!-- Instruments -->
<h5><span style="background-color:#23b4f9; color:white; padding: 10px; border-radius:10px 10px 0 0;">Instruments</span></h5>

**Instruments** 是一个包含在 **Xocde** 工具内的，强大灵活的**苹果应用程序性能优化和测试工具**。用它来收集关于一个或多个系统进程的性能和行为的数据极为方便，并能及时跟踪随着时间产生的数据，还可以广泛收集不同类型的数据。虽然 **ARC (Automatic Reference Counting)** 机制可以帮你做很多工作，而且你也努力地去避免，但是最后还是会出现 **memory leak (内存泄漏)**。所以在你的软件开发工作流中尽早地使用 **Instruments** 可以帮你节省时间，缩短开发周期。

如何打开 **Instruments** 呢? 首先打开 **Xcode**，然后选择 `Xcode > Open Developer Tool > Instruments`。

<span style="border:2px solid #23b4f9; padding:5px; border-radius:10px"><b>参考资料：</b></span>

[Instruments User Guide](https://developer.apple.com/library/prerelease/content/documentation/DeveloperTools/Conceptual/InstrumentsUserGuide/index.html#//apple_ref/doc/uid/TP40004652-CH3-SW1) <br>
[Finding iOS Memory Leaks with Xcode’s Instruments](https://spin.atomicobject.com/2016/01/25/ios-memory-leak-xcode/) <br>
[iOS性能优化](http://www.jianshu.com/p/9e1f0b44935c)
<br><br>

<!-- MapKit -->
<h5><span style="background-color:#23b4f9; color:white; padding: 10px; border-radius:10px 10px 0 0;">MapKit</span></h5>

**MapKit** 是一个苹果软件开发 **framework (框架)**，它提供了把地图直接嵌入到 **windows (窗口)** 和 **views (视图)** 的 **interface (界面)**。它同时支持在地图上**注释，添加覆盖层，逆向地理编码** — 将映射坐标转换成实际位置等功能。

<span style="border:2px solid #23b4f9; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[MapKit Framework Reference](https://developer.apple.com/library/mac/documentation/MapKit/Reference/MapKit_Framework_Reference/)
<br><br>

<!-- CoreData -->
<h5><span style="background-color:#23b4f9; color:white; padding: 10px; border-radius:10px 10px 0 0;">CoreData</span></h5>

**CoreData** 是一个苹果软件开发 **framework (框架)**，它使你能够处理应用程序中 **model layer (模型层)** 的 **objects (对象)**。它提供了和 **object life cycle (对象生命周期)** 有关的(包括对象持久化，意即存储)，普适的，自动的解决方案。

**CoreData** 所包含的内建功能可以帮你减少 50% 到 70% 的为 **model layer (数据模型层)** 而写的代码。

<span style="border:2px solid #23b4f9; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[What Is Core Data?](https://developer.apple.com/library/watchos/documentation/Cocoa/Conceptual/CoreData/index.html)
<br><br>

<!-- --------------------------------------- -->

<h3 id="front">Web 前端开发</h3>

<!-- HTML -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">HTML</span></h5>

全称 **HyperText Markup Language**，**超文本标记语言** 一种用于创建网页的标准标记语言，可以理解为一种表示**内容**和**语义**的**数据封装格式**。

**HTML** 文件扩展名为 `.html` 或者 `.htm`。

<!-- XML -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">XML</span></h5>

全称 **eXtensible Markup Language**，**可扩展标记语言**，是一种标记语言。标记指计算机所能理解的信息符号，通过此种标记，计算机之间可以处理包含各种信息的文章等。标记语言就是用来约定这些标记的，**HTML** 是国际通用的标记语言，**XML** 则是可以由相关人士自由定制的标记语言，因此说它是可扩展标记语言。**XML** 是从标准通用标记语言（SGML）中简化修改出来的。 

* HTML 被设计用来显示数据，其焦点是数据的外观。
* XML 被设计为传输和存储数据，其焦点是数据的内容。
* XML 标签没有被预定义。您需要自行定义标签。
* XML 被设计为具有自我描述性。

**XML** 文件扩展名为 `.xml`。

<!-- XHTML -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">XHTML</span></h5>

全称 **eXtensible HyperText Markup Language**，是一种标记语言，表现方式与 **HTML** 类似，不过**语法上更加严格**。从继承关系上讲，HTML 是基于标准通用标记语言（SGML）的，而 **XHTML** 则基于XML，而且 XHTML 为了兼容 XML 语法上和 HTML 有些不同。

可以理解为：**XHTML 是更严谨更纯净的 HTML 版本**。

**XHTML** 文件扩展名为 `.xhtml` 或 `.xht` 或 `.xml` 或 `.html` 或 `.htm`。

<!-- Markdown -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">Markdown</span></h5>

**Markdown** 是一种轻量级标记语言。它允许人们 "使用易读易写的纯文本格式编写文档，然后转换成有效的 XHTML (或者 HTML)文档"。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。

**Markdown** 文件扩展名为为 `.markdown` 或者 `.md`。

<!-- YAML -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">YAML</span></h5>

**YAML** 是一个可读性高，用来表达资料序列的格式，或者说一种通用的**数据串行化格式**。

**YAML** 是 **YAML Ain't a Markup Language**（YAML不是一种标记语言）的递归缩写。在开发这种语言时，**YAML** 最早的意思是 **Yet Another Markup Language**（仍是一种标记语言），后来为了强调这种语言**以数据作为中心**，而不是以标记语言为重点，才采用反向缩略语重新命名。

**YAML** 參考了 JSON，XML 和 SDL 等语言，不过跟这些语言比起来，YAML仍有自己的特色。**YAML 用来写配置文件，非常简洁和强大，比 JSON 方便**。

**YAML** 文件扩展名为 `.yaml` 或者 `.yml`。

<!-- JSON -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">JSON</span></h5>

全称 **JavaScript Object Notation**，**JavaScript 对象表示法**，是一种轻量级的数据交换格式，存储和交换文本信息的语法。类似XML。**JSON** 比 XML 更小、更快，更易解析。**JSON** 使用 JavaScript 语法来描述数据对象，但是 JSON 仍然是独立于语言和平台的文本格式，并且采用了 C 语言家族的一些习惯。JSON 解析器和 JSON 库支持许多不同的编程语言。

<!-- CSS -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">CSS</span></h5>

全称 **Cascading Style Sheets**，层叠样式表，是一种样式表标记语言，用于为HTML文档定义布局。 例如，CSS涉及字体、颜色、边距、高度、宽度、背景图像、高级定位等方面。

<!-- SASS -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">SASS</span></h5>

全称 **Syntactically Awesome Style Sheets**，一种 Ruby 写的 **层叠样式表语言**，将脚本解析成 CSS 的脚本语言，即 SassScript。

> 学过 CSS 的人都知道，它不是一种编程语言。你可以用它开发网页样式，但是没法用它编程。也就是说，CSS 基本上是设计师的工具，不是程序员的工具。在程序员眼里，CSS 是一件很麻烦的东西。它没有变量，也没有条件语句，只是一行行单纯的描述，写起来相当费事。

> 很自然地，有人就开始为 CSS 加入编程元素，这被叫做 **"CSS 预处理器"（CSS preprocessor）**。它的基本思想是，用一种专门的编程语言，进行网页样式设计，然后再编译成正常的 CSS 文件。

**SASS** 文件扩展名为 `.sass` 或者 `.scss`。

<span style="border:2px solid #f9b955; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[SASS用法指南](http://www.ruanyifeng.com/blog/2012/06/sass.html)
<br><br>

<!-- LESS -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">LESS</span></h5>

**LESS** 是一种**动态层叠样式表语言**，受 SASS 所影响，同时也影响了 SASS 的新语法：SCSS。所以和 SASS 一样也可以理解为一种 **CSS 预处理器**。

**LESS** 是开源的，其第一个版本由 Ruby 写成，但在后续的版本当中，Ruby 逐渐被替换为 JavaScript。受益于 JavaScript，LESS 可以在客户端上运行（IE6+、Webkit、Firefox），也可以在服务器端运行（Node.js、Rhino）。

在语法方面，**LESS** 与 CSS 较为接近，一个合法的 CSS 代码段本身也是一段合法的 LESS 代码段。LESS 提供变量、嵌套、混合、操作符、函数等一般编程所需的抽象机制。

<!-- JavaScript -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">JavaScript</span></h5>

**JavaScript** 和 **Java** 的关系，就像北大和北大青鸟之间的关系一样，没什么太大关联。**JavaScript** 并不是解释型的 Java 语言。Java 是解释型的高级汇编语言，**JavaScript** 是另一种语言。**JavaScript** 和 Java 的语法很相似，就象 Java 和 C 的语法相似一样。

**JavaScript** 并不是由 Sun公司 ── Java 的老家──开发的。**JavaScript** 是由 **Netscape**公司开发。它本来叫做 **LiveScript**，后来 **Netscape为了搭上媒体热炒 Java 的顺风车，所以改名为 Javascript**。

* **JavaScript** 是世界上最流行的**脚本语言**。(Script 其实指的是不需要编译就可以运行的一系列指令，用来自动化地完成机械性重复性的工作)
* **JavaScript** 是属于 Web 的语言，它适用于 PC、笔记本电脑、平板电脑和移动电话。
* **JavaScript** 可以**实现动态效果**，动态**改变网页内容**，实现和用户的操作进行**交互**，使一些工作在**本地完成**减轻服务器负担。
* 许多 HTML 开发者都不是程序员，但是 **JavaScript** 却拥有非常简单的语法。几乎每个人都有能力将小的 **JavaScript** 片段添加到网页中。

<!-- AJAX -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">AJAX</span></h5>

全称 **Asynchronous JavaScript and XML**，**异步的 JavaScript 和 XML**。
**AJAX** 不是新的编程语言，而是一种使用现有标准的新方法。
**AJAX** 是在不重新加载整个页面的情况下与服务器交换数据并更新部分网页的技术。

所谓**异步**，简单地解释就是：向服务器发送请求的时候，我们不必等待结果，可以同时做其他的事情，等到有了结果我们可以再回去处理。如果不是**异步**的话，我们点完按钮，页面就会死在那里，其他的数据请求不会往下走了。**XML** 只是一种**数据封装格式**，我们在更新一行字的时候理论上说不需要这个格式，但如果我们更新很多内容，那么格式化的数据可以使我们有条理地去实现更新。现在大部分人其实是用 **JSON** 这种格式来代替 **XML** 的，因为 **JSON** 更加简洁，据说目前的解析速度也更快。

<!-- Node.js -->
<h5><span style="background-color:#f91600; color:white; padding: 10px; border-radius:10px 10px 0 0;">Node.js</span></h5>

> **Node.js** is an open-source, cross-platform **runtime environment** for developing **server-side Web applications**. Although **Node.js is not a JavaScript framework**, many of its basic modules are written in **JavaScript**, and developers can write new modules in JavaScript. The runtime environment interprets JavaScript using **Google's V8 JavaScript engine**.

**Node.js** 不是 JavaScript 应用，而是 **JavaScript 运行平台**。Node.js 采用 C，C++，JavaScript 语言编写而成，是一个开放源代码、跨平台的、可用于服务器端和网络应用的 **JavaScript 的运行环境**，或者说 **服务器端 JavaScript 解释器**。

**Node.js** 是一个 **后端的** JavaScript 运行环境，**这意味着你可以编写系统级或者服务器端的 JavaScript 代码，交给 Node.js 来解释执行**，简单的命令类似于：`#node helloworld.js`

**Node.js** 采用了 Google Chrome浏览器的V8引擎，性能很好，同时还提供了很多系统级的API，如文件操作、网络编程等。浏览器端的 Javascript 代码在运行时会受到各种安全性的限制，对客户系统的操作有限。相比之下，**Node.js** 则是一个全面的后台运行时，为 Javascript 提供了其他语言能够实现的许多功能。

> 小贴士：在Mac机上推荐用 **Homebrew** 安装 **Node.js**，npm 指的是 **Node Package Manager** (Node的模块管理器)。

<span style="border:2px solid #f91600; padding:5px; border-radius:10px"><b>参考资料：</b></span>

[Node.js](https://en.wikipedia.org/wiki/Node.js) <br>
[深入浅出 Node.js：什么是 Node.js](http://www.infoq.com/cn/articles/what-is-nodejs)
<br><br>

<!-- Gulp -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">Gulp</span></h5>

**Gulp** 是基于 Node.js 的**自动任务运行器**，她能自动化地完成 javascript/coffee/sass/less/html/image/css 等文件的的测试、检查、合并、压缩、格式化、浏览器自动刷新、部署文件生成，并监听文件在改动后重复指定的这些步骤。

<!-- Grunt -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">Grunt</span></h5>

**Grunt** 是基于 Node.js 的**项目构建工具**。它可以**自动运行你所设定的任务**。**Grunt** 拥有数量庞大的插件，几乎任何你所要做的事情都可以用 **Grunt** 实现。

> **Gulp** 和 **Grunt** 是同一类自动化工具，关于区别和优劣，请参看下面的参考资料。

<span style="border:2px solid #f9b955; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[Gulp挑战Grunt，背后的哲学](http://www.jianshu.com/p/3779f708f5d7)
<br><br>

<!-- Bower -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">Bower</span></h5>

**Bower** 是一个用于管理前端依赖的 **包管理器（Package Manager）**，该开源项目由 Twitter 创建。 与此相对应的包括，PHP 的 Composer ，Node 的 **NPM (Node Package Manager)**，和 Ruby 的 RubyGems 。

<!-- Jade -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">Jade</span></h5>

**模板引擎**是用来动态渲染**模板文件**并输出为可被浏览器识别的**HTML文件**，**Node** 中常用的模板引擎有 **Jade** 和 **Ejs**。

**Jade** — Node Template Engine 是一个高性能的**模板引擎**，为 Node 而做，用 JavaScript 实现。
Node.js 的 Express.js 框架默认用的就是 Jade。**Jade** 还有其他语言的实现，可以实现前后端渲染的统一。比如 php、ruby、python、java、scala。

<span style="border:2px solid #f9b955; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[Jade中文教程](http://blog.jayself.com/2014/07/28/Jade/)
<br><br>

<!-- Liquid -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">Liquid</span></h5>

> **Liquid** is an open-source **template language** created by Shopify and written in Ruby. It is the backbone of Shopify themes and is used to load dynamic content on storefronts.

**模板引擎**是 Web应用 中用来生成动态HTML的工具， 它负责将数据模型与 HTML 模板结合（模板渲染），生成最终的 HTML。 编写 HTML模板 的语法称为**模板语法**，模板语法的表达能力和可扩展性决定了模板引擎的易用性。

> Jade is a **template language**.

和 **Jade** 一样 **Liquid** 也是一种**模板语言**。

<span style="border:2px solid #f9b955; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[Liquid 是世界上最好的模板引擎](http://harttle.com/2016/06/27/shopify-liquid.html)
<br><br>

<!-- BootStrap -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0; border:2px solid #000000;">BootStrap</span></h5>

**Bootstrap** 是两个 Twitter 员工开发并开源的用于快速开发 **Web 应用程序**和**网站**的 前端 **framework (框架)**，目前很受欢迎。Bootstrap 是基于HTML、CSS、JavaScript 的。

<!-- Meteor.js -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0; border:2px solid #000000;">Meteor.js</span></h5>

> Meteor is an open-source platform for building top-quality web apps in a fraction of the time, whether you're an expert developer or just getting started.

**Meteor.js** 是一个 **Web App** 开发 **framework (框架)**，你只需要使用 **HTML + CSS + JavaScript** 就可以独立开发一个跨平台的 Web App。你可以轻松完成全栈式开发的所有工作，注意是**轻松**完成。

**Meteor.js** 构架于 **Node.js** 之上。这使得 One Language 成为可能，同时可依托 **Node.js** 上诸如 <http://socket.io> 这样强大的类库内置 realtime，date on the wire 等特性。

在一种语言的基础上，**Meteor.js 统一了服务器端和客户端的数据访问**，提出 Database Everywhere，一套 DateBase API 大大减轻了开发负担，不用再做 server data JSON client data 的转换。

<!-- Angular.js -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0; border:2px solid #000000;">Angular.js</span></h5>

**Angular.js** 是一个来自 Google 的 前端 JavaScript **framework (框架)**。 它可通过 `<script>` 标签添加到 HTML 页面。 **Angular.js** 通过指令扩展了HTML，且通过表达式绑定数据到HTML。

**Angular.js** 最适于开发客户端的单页面应用。它不是个功能库，而是用来**开发动态网页的框架**。它专注于扩展HTML的功能，提供动态数据绑定（data binding），而且它能跟其它框架（如jQuery）合作融洽。

<!-- React.js -->
<h5><span style="background-color:#49d682; color:white; padding: 10px; border-radius:10px 10px 0 0;">React</span></h5>

> **React** is an open-source **JavaScript library** providing a view for data rendered as HTML, for building **user interfaces**.

**React** 是 Facebook 开发的一款 **JavaScript 库**。

* React 不是一个 MVC 框架，它是构建易于可重复调用的 web组件，侧重于 UI, 也就是 view 层。
* 其次 React 是单向的从数据到视图的渲染，非双向数据绑定。
* 不直接操作 DOM 对象，而是通过虚拟 DOM 通过 diff算法 以最小的步骤作用到真实的 DOM 上。
* 不便于直接操作 DOM，大多数时间只是对 virtual DOM 进行编程。

<!-- jQuery -->
<h5><span style="background-color:#49d682; color:white; padding: 10px; border-radius:10px 10px 0 0;">jQuery</span></h5>

**jQuery** 是一种快速简洁的 **JavaScript 库**，它的理念是用更少的代码，实现更多的功能。 **jQuery** 简化了  HTML 文档遍历、事件处理、动画以及 Ajax 交互，用于快速 web 开发。

<!-- JavaScript 框架和库有什么关系和区别 -->
* JavaScript **framework (框架)** 和 **library (库)** 有什么关系和区别?

> Your code calls a **library** but a **framework** calls your code. Framework contains library.

**Framework (框架)** 倾向于提供整套的解决方案，倾向于创造一些需要你来遵守的规则和范例。比如 AngularJS 就算是一个框架，因为它提供了一整套的解决方案，需要你按照它设计好的方式来写代码。

<!-- --------------------------------------- -->

<h3 id="end">Web 后端开发</h3>

<!-- PHP -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0;">PHP</span></h5>

**PHP**（"PHP: Hypertext Preprocessor"，**超文本预处理器**的字母缩写）是一种被广泛使用的开源脚本语言，它可嵌入到 HTML 中，尤其适合 Web 开发。PHP 脚本在 **服务器上执行**。PHP 没有成本，可供免费下载和使用。

* PHP 文件能够包含文本、HTML、CSS 以及 PHP 代码<br>
* PHP 易于学习，并可高效地运行在**服务器端**，而结果以**纯文本**形式返回浏览器<br>
* PHP 能够生成动态页面内容<br>
* PHP 能够创建、打开、读取、写入、删除以及关闭服务器上的文件<br>
* PHP 能够接收表单数据，能够发送并取回 cookies <br>
* PHP 能够添加、删除、修改数据库中的数据，并能够对数据进行加密<br>
* PHP 能够限制用户访问网站中的某些页面<br>
* 通过 PHP 能够输出 HTML、图像、PDF、甚至 Flash 影片。也可以输出任何文本，比如 XHTML 和 XML<br>
* PHP 运行于各种平台：Windows, Linux, Unix, Mac OS X 等等<br>
* PHP 兼容几乎所有服务器：Apache, IIS 等等<br>
* PHP 支持多种数据库<br>

**PHP** 文件的扩展名是 `.php`。

**JavaScript** 是工作在**浏览器端的脚本语言**，他所提交的数据是交给浏览器来处理的。但是现在的 Ajax 技术已经可以把 JS 提交的数据交付到服务器来处理。**PHP**，是工作在**服务器端的脚本语言**，把数据提交给服务器去处理，服务器再响应到浏览器。一个是**服务器端脚本**，一个是**客户端脚本**。单纯用服务器端脚本实现某些功能的话，交互界面会很不友好 (数据传输需要提交到服务器，会刷新页面)。
JS 可以在浏览器中直接操作页面，但是单纯 JS 的话是没有数据持久化能力的，一旦清空了浏览器数据，就什么都没有了。

<span style="border:2px solid #f9b955; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[PHP 简介](http://www.w3school.com.cn/php/php_intro.asp)
<br><br>

<!-- Symfony -->
<h5><span style="background-color:#f9b955; color:white; padding: 10px; border-radius:10px 10px 0 0; border:2px solid #000000;">Symfony</span></h5>

> Symfony is a set of reusabable PHP Components, a Web Application framework, a Philosophy, and a Community — all working together in harmony.

**Symfony** 是一款开源的基于 **MVC架构** 的，面向对象的 PHP **framework (框架)**。

<span style="border:2px solid #f9b955; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[Symfony](https://symfony.com/)
<br>

<!-- --------------------------------------- -->

<h3 id="dataBase">数据库</h3>

> **Database (数据库)**，简单来说就是储存电子档案的处所，使用者可以对档案中的资料执行新增、摘取、更新、刪除等操作。 **数据库**指的是以一定方式储存在一起、能为多个用户共享、具有尽可能小的冗余度、与应用程序彼此独立的**数据集合**。

<!-- SQL -->
<h5><span style="background-color:#6de0c2; color:white; padding: 10px; border-radius:10px 10px 0 0;">SQL</span></h5>

全称 **Structural Query Language**，**结构化查询语言**，用于数据库中的标准数据查询的语言，最早由IBM公司使用在其开发的数据库系统中。各种通行的数据库系统在其实践过程中都对 **SQL** 规范作了某些编改和扩充。所以，实际上不同数据库系统之间的 **SQL** 不能完全相互通用。

**SQL** 文件的扩展名是 `.sql`。

<!-- Microsoft SQL Server -->
<h5><span style="background-color:#9f99e0; color:white; padding: 10px; border-radius:10px 10px 0 0;">Microsoft SQL Server</span></h5>

微软的 **RDBMS (Relational DataBase Manager System)**，**关联式数据库管理系统**。

<!-- MySQL -->
<h5><span style="background-color:#9f99e0; color:white; padding: 10px; border-radius:10px 10px 0 0;">MySQL</span></h5>

一个开源的 RDBMS，**关联式数据库管理系统**。原开发者為瑞典的 MySQL AB 公司，该公司于2008年被升阳微系統（Sun Microsystems）收购。2009年，甲骨文公司（Oracle）收购升阳微系統公司，MySQL 成为 Oracle 旗下产品。

<!-- SQLite -->
<h5><span style="background-color:#9f99e0; color:white; padding: 10px; border-radius:10px 10px 0 0;">SQLite</span></h5>

**SQLite** 是一种**关系型数据库管理系统**，它包含在一个相对小的C程式庫中。与许多其它数据库管理系统不同，**SQLite** 不是一个客户端/服务器结构的数据库引擎，而是被**集成在用户程序中**。**SQLite** 遵守 ACID，实现了大多数 SQL 标准。它使用动态的、弱类型的 SQL 语法。它作为嵌入式数据库，是应用程序，如网页浏览器，在本地/客户端存储数据的常见选择。

<!-- NoSQL -->
<h5><span style="background-color:#e07125; color:white; padding: 10px; border-radius:10px 10px 0 0;">NoSQL</span></h5>

**NoSQL** 是对**不同于传统的关联式数据库管理系统的统称**。**NoSQL** 不使用 SQL 作為查询语言。其数据存储可以不需要固定的表格模式，也经常会避免使用 SQL 的 JOIN 操作，一般有水平可扩展性的特征。**NoSQL** 的实现具有二个特征：使用硬碟，或者把随机存储器作存储载体。

<span style="border:2px solid #e07125; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[What is NoSQL?](https://www.mongodb.com/nosql-explained)
<br><br>

<!-- MongoDB -->
<h5><span style="background-color:#ead078; color:white; padding: 10px; border-radius:10px 10px 0 0;">MongoDB</span></h5>

**MongoDB** 是 10gen 这家公司开发的一個 NoSQL Database，是一种开源高性能的 **Document-Oriented Database (文档型数据库)**。它旨在结合 Relational Database 与 Key/Value Database 双方的优点，适合用在 Web 应用程式。

<!-- Realm -->
<h5><span style="background-color:#ead078; color:white; padding: 10px; border-radius:10px 10px 0 0;">Realm</span></h5>

> **Realm** is a **mobile database**: a replacement for SQLite & ORMs & CoreData & key-value stores.

<span style="border:2px solid #ead078; padding:5px; border-radius:10px"><b>参考资料：</b></span>
[A better mobile database means better apps.](https://realm.io)

<h3 id="tip">小窍门</h3>
Mac Terminal 内输入 `ls -a` 可以在 Terminal 里列出隐藏文件并保证桌面上不显示。

##### 著作权声明

所有资料来源于网络，内容版权均归原作者所有，本文由 Theo 独家整理，转载请保留原文链接，谢谢。
