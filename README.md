#Theo's Blog

###[View Live Theo's Blog &rarr;](http://theowu.github.io)

![](http://theowu.tk/img/blog-desktop.jpg)

## Features

Theme coloned from [Hux Blog](https://github.com/huxpro/huxpro.github.io/)
Below are features of historical versions:

##### New Feature (V1.5.1)

- **[Comment](#comment)** support [**Disqus**](http://disqus.com) officially, thanks to @rpsh.

##### New Feature (V1.5)

- **[Comment](#comment)** and **[Analytics](#analytics)** is configurable now! We also add **Google Analytics support** and drop tencents. Both documents is updated.

##### New Feature (V1.4)

- **[Featured Tags](#featured-tags)** is now independent of [SideBar](#sidebar). Both documents is updated.
- New **[SEO Title](#seo-title)** for SEO usage which is differ from the site title

##### New Feature (V1.3.1)

- Support **PingFang (苹方)**, the new Chinese font presented by [OS X El Capitan](http://www.apple.com/cn/osx/whats-new/)


##### New Feature (V1.3)

- Big Improvement to the **Navigation Menu** *(especially in Android)*:  Dropping the old, stuttering, low-performance [Bootstrap collapse.js](http://getbootstrap.com/javascript/#collapse),  replaced with an own wrote, [jank free](http://jankfree.org/) navbar menu in a pretty high-performance implementation of [Google Material Design](https://www.google.com/design/spec/material-design/introduction.html).

<img src="http://theowu.tk/img/blog-md-navbar.gif" width="320" />


##### New Feature (V1.2)

- Brand new **[Keynote Layout](#keynote-layout)** is provided for easily posting beautiful HTML presentations you have created with this blog


##### New Feature (V1.1)

- We now support a clean and gorgeous **[SideBar](#sidebar)** for displaying more info
- **[Friends](#friends)** is also added as a common feature of blog help you do SEO

##### V1.0

- Full-feature **Tag** support
- **Mobile first** user experience optimization
- **Typographic optimization** for Chinese Fonts
- **Network optimizaition** for China, dropping Google webfont, using local CDN
- Using [Github Flavored Markdown](https://help.github.com/articles/github-flavored-markdown/)
- Using Baidu, Tencent/QQ analytics
- Using [DuoShuo](http://duoshuo.com/) as the Disqus-like third party discussion system


## Support

- **Feel free to fork or clone. I'll Appreciate it if you keep the Author & Github link at footer**
- Give it a **Star** if you like, fork or just clone to use ;)


## Document

* Get Started
	* [Environment](#environment)
	* [Get Started](#get-started)
	* [Write Posts](#write-posts)
* Components
	* [SideBar](#sidebar)
	* [Mini About Me](#mini-about-me)
	* [Featured Tags](#featured-tags)
	* [Friends](#friends)
	* [Keynote Layout](#keynote-layout)
* Comment & Analysis
	* [Comment](#comment)
	* [Analytics](#analytics)
* Advanced
	* [Customization](#customization)
	* [Header Image](#header-image)
	* [SEO Title](#seo-title)
	* [Page Build Warning](#page-build-warning)

#### Environment

If you have jekyll installed, simply run `jekyll serve` in Command Line
and preview the themes in your browser. You can use `jekyll serve --watch` to watch for changes in the source files as well.


#### Get Started

You can easily get started by modifying `_config.yml`:

```
# Site settings
title: Theo's Blog          # title of your website
SEOTitle: Theo's Blog		# check out docs for more detail
description: "Cool Blog"    # write something to describe your website

# SNS settings      
github_username: theowu     # modify this account to yours
weibo_username: 1919490675  # the footer woule be auto-updated.

# Build settings
# paginate: 10              # nums of posts in one page, in this case, 10
```

There are more options you can check out in the [Jekyll - Official Site](http://jekyllrb.com/), or you can directly dive into code to find more.


#### Write Posts

Feel free to checkout Markdown files in the `_posts/`, you will quickly realized how to post your articles with magical markdown plus this nice theme.

The **front-matter** of a post looks like that:

```
---
layout:     post
title:      "Hello 2016"
subtitle:   "Hello World, Hello Jekyll"
date:       2015-01-29 12:00:00
author:     "Thep"
header-img: "img/post-bg/2016-08-16-hello-2016.jpg"
tags:
    - Life
---

```

#### SideBar

![](http://theowu.tk/img/blog-sidebar.jpg)

Seeing more information may be necessary for you to display, from V1.1, a clean, gorgeous **SideBar** is added for you, which provide more area for displaying possible modules. You can enable *(it is default enable)* this feature by simply config:

```
# Sidebar settings
sidebar: true
sidebar-about-description: "your description here"
sidebar-avatar: /img/avatar-theo.jpg     # please use absolute URL.
```

We default support *[Featured Tags](#featured-tags)*, *[Mini About Me](#mini-about-me)* and *[Friends](#friends)* these three modules and you can add your own. The sidebar is naturally responsive and would be push to bottom in a small screen size (`<= 992px`, according to [Bootstarp Grid System](http://getbootstrap.com/css/#grid))  
More details of these three separate modules are talking below.

#### Mini About Me

Mini-About-Me module display all your SNS buttons also your avatar and the description if you set `sidebar-avatar` and `sidebar-about-description` which is very useful and common for a sidebar so it is default with your sidebar.

It is really nice-looking and well-designed. It would be hidden in a small screen seeing the sidebar would be push to bottom and there is already a footer including SNS feature which is similar.

#### Featured Tags

Considering the Featured-Tags feature in [Medium](http://medium.com) is pretty cool, so I add it in my blog theme also.   
This module is independent of sidebar from V1.4, so it can definitely live without enable sidebar, which would be displayed in the bottom when `sidebar` set to false, and it is not only displayed in home page but also every post page bottom.


```
# Featured Tags
featured-tags: true  
featured-condition-size: 1     # A tag will be featured if the size of it is more than this condition value
```

The only one thing need to be paid attention to is the `featured-condition-size`: A tag will be featured if the size of it is more than this condition value.  
Internally, a condition template `{% if tag[1].size > {{site.featured-condition-size}} %}` is used to do the filter.

#### Friends

Friends is a very common feature of a blog seeing the SEO, so Huxpro add it in V1.1 release to help that.   
Friends can also live without enable sidebar, also be displayed in the bottom when sidebar unable, and be displayed in every post page bottom.


You can just add your friends information in `_config.yml` with a familiar JSON syntax and everything is done, very easy:

```
# Friends
friends: [
    {
        title: "Theo's Blog",
        href: "http://theowu.github.io/"
    },
    {
        title: "Foo Blog",
        href: "http://foo.github.io/"
    },
    {
        title: "Bar Blog",
        href: "http://bar.github.io"
    }
]
```


#### Keynote Layout

![](http://theowu.tk/img/blog-keynote.jpg)

There is a increasing tendency to use Open Web technology to create keynotes, presentations, like Reveal.js, Impress.js, Slides, Prezi etc. I consider a modern blog should have abilities to post these HTML based presentation easily also abilities to play it directly.

Under the hood, a `iframe` is used to include webpage from outer source, so the only things left is to give a url in the **front-matter**:

```
---
layout:     keynote
iframe:     "http://theowu.tk/js-module-7day/"
---
```

The iframe will be automatically resized to adapt different form factors also the device orientation. A padding is left to imply user that there has more content below, also to ensure that there is a area for user to scroll down in mobile device seeing most of the keynote framework prevent the browser default scroll behavior.


#### Comment

This theme support both [Disqus](http://disqus.com) and [Duoshuo](http://duoshuo.com) as the third party discussion system.

First, you need to sign up and get your own account. **Repeat, DO NOT use mine!** (I have set Trusted Domains), otherwise, you will have problems. It is deathly simple to sign up and you will get the full power of management system. Please give it a try!

Second, thanks to huxpro, from V1.5, you can easily complete your comment configuration by just adding your **short name** into `_config.yml`:

```
duoshuo_username: _your_duoshuo_short_name_
# OR
disqus_username: _your_disqus_short_name_
```

**To the old version user**, it's better that you pull the new version, otherwise you have to replace code in `post.html`, `keynote.html` and `about.html` by yourselves.

Furthermore, Duoshuo support Sharing. if you only wanna use Duoshuo comment without sharing, you can set `duoshuo_share: false`. You can use Duoshuo Sharing and Disqus Comments together also.



#### Analytics

From V1.5, we support Google Analytics and Baidu Tongji officially with a deathly simple config:

```
# Baidu Analytics
ba_track_id: 4cc1f2d8f3067386cc5cdb626a202900

# Google Analytics
ga_track_id: 'UA-49627206-1'            # Format: UA-xxxxxx-xx
ga_domain: huangxuan.me
```

Just checkout the code offered by Google/Baidu, and copy paste here, all the rest is already done for you.

#### Customization

If you wanna do more customization and change code yourself, a [Grunt](gruntjs.com) environment is also included. (Thanks to the famous Clean Blog.)

There are a number of tasks it performs like minification of the JavaScript, compiling of the LESS files, adding banners to keep the Apache 2.0 license intact, and watching for changes. Run the grunt default task by entering `grunt` into your command line which will build the files. You can use `grunt watch` if you are working on the JavaScript or the LESS.

**Try to understand code in `_include/` and `_layouts/`, then you can modify Jekyll [Liquid](https://github.com/Shopify/liquid/wiki) template directly to do more creative customization.**


#### Header Image

Change header images of any pages or any posts is pretty easy as mentioned above. It can be done in every post you write in your favorite markdown or html language.

#### SEO Title

Before V1.4, site setting `title` is not only used for displayed in Home Page and Navbar, but also used to generate the `<title>` in HTML.
It's possible that you want the two things different. For me, my site-title is **“Theo's Blog”** but I want the title shows in search engine is **“吴思元的博客 | Theo's Blog”** which is multi-language.

So, the SEO Title is introduced to solve this problem, you can set `SEOTitle` different from `title`, and it would be only used to generate HTML `<title>` and setting DuoShuo Sharing.

#### Page Build Warning

There are many possible reasons to cause a "Page Build Warning" email or similar error.

One of these is that github changes its build environment.

> You are attempting to use the 'pygments' highlighter, which is currently unsupported on GitHub Pages. Your site will use 'rouge' for highlighting instead. To suppress this warning, change the 'highlighter' value to 'rouge' in your '_config.yml'.

So, just edit `_config.yml`, find `highlighter: pygments`, change it to `highlighter: rouge` and the warning will be gone.

For other circumstance, check out existing issues or create a new one!

## Porting 

- [**Hexo**](https://github.com/Kaijun/hexo-theme-huxblog) by @kaijun
- [**React-SSR**](https://github.com/LucasIcarus/huxpro.github.io/tree/ssr) by @LucasIcarus

## Thanks

This theme is cloned from [Hux Blog](https://github.com/huxpro/huxpro.github.io/) which is forked from [IronSummitMedia/startbootstrap-clean-blog-jekyll](https://github.com/IronSummitMedia/startbootstrap-clean-blog-jekyll). Special thanks to these people.  

Thanks Jekyll and Github Pages!
