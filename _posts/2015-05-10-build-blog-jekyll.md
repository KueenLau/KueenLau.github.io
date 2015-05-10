---
layout: post
title: "手把手教你用Github搭建独立博客（四）"
date: 2015-05-10 7:30:00
categories: blog-build
featured_image: /images/cover.jpg
---
##Jekyll Introduction&configuration

　　首先介绍一下jekyll是干什么的。它是一个博客生成工具，功能强大但是又简单易

操作。你只需要在本地用html/css+markdown标记语言配上liquid的流程控制就能通过

jekyll生成静态页面了，注意jekyll是只能生成静态页面的，也就是说例如动态的目录导

航或者其他的动态功能就只能考虑使用插件了。

###安装jekyll

[jekyll-windows.juthilo.com/](http://jekyll-windows.juthilo.com/)关于jekyll需要的环境以及所有的安装过程大家只要按照左边

链接上的步骤一步一步完成就行了。

###jekyll目录结构

大家应该还对我本地文件的目录结构有印象，发现里面的文件夹及文件都有固定的取名方式

![本地文件结构](http://i1.tietuku.com/ed78f8e4ec78e965.png)

这里面的文件组织结构都是严格按照jekyll的设定来建立的，现在就简单介绍一下

各文件的作用。

_layouts文件夹主要存放博客的页面外观代码，一般会有default.html和post.html。

_plugins文件夹主要存放一些外部插件的代码。

_posts文件夹主要存放博客的文章内容文件，比如markdown文件或者txt文件。

_site文件夹里就是当你运行站点之后整个网站所包含的所有文件。

_config.yml是jekyll配置文件，里面包括的信息有很多，譬如你站点的编码方式、默认的

页面样式等等。

以上是最主要的几个文件，当然还有其他的很多文件，但都不是必须的，你可以参照


[http://jekyll.bootcss.com/](http://jekyll.bootcss.com/)。

###jekyll使用方法

在你的文件根目录上运行任何的shell，然后键入：

    $ jekyll build --watch


这样jekyll就能将你的所有站点信息加入到_site文件里，同时监视着任何产生的文件修改。

如果想要在本地调试你的博客，jekyll也提供了一个本地服务器的功能，在command shell

里面输入:

    $ jekyll serve

然后在浏览器访问本地4000端口（jekyll默认的）就能进行页面显示，非常方便调试。

###jekyll模板

github上现在有很多现成的jekyll模板，如果你觉得自己一行行代码建站麻烦，还可以选择直接

将模板fork后pull到本地，会省去不少功夫。链接——>[https://github.com/jekyll/jekyll/wiki/Sites](https://github.com/jekyll/jekyll/wiki/Sites)

选择一个简洁又好看的模板对你博客的人气也会大有帮助哦！~