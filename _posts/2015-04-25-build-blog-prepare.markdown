---
layout: post
title: "手把手教你用Github搭建独立博客（二）"
date: 2015-04-25 9:58:00
categories: experience
featured_image: /images/cover.jpg
---
##Preliminary

　　在进行博客搭建之前，我们需要做一些准备工作：1.购买一个域名，2.注册一个DNS

服务商的账号，3.注册一个Github账号。

   **购买域名:**

　　你可以在百度上键入“域名购买”，然后就会有很多域名注册的网站，随便选择一个就是

啦。本人使用的是[耐思尼克](http://www.iisp.com/)提供的域名。

　　进入该网站后先进行注册然后登录。在输入框内输入你想要的域名，这个域名就相当于你

在万维网里的名字一样，所以有没有特点容不容易被人记住就很重要啦。

![域名注册](http://i1.tietuku.com/eb3336874a3f2b57.png)

　　接着就很easy了，完全是点一点鼠标就能完成的了，当然还需要掏一掏你的钱包。

![域名购买](http://i1.tietuku.com/001ce60cf7b02131.png)

　　这样，你就买到了你自己的“网络代号”了。不要忘记上传自己的身份证照片进行验证，否则

7天之后就会把你的域名给停用了。

**Github:**

　　[Github](https://github.com)是个很nice的东西，你可以把你任何想放的比如代码、文档等等一股脑地往上面扔。

![Github注册](http://i1.tietuku.com/be42f3891a307f01.png)

先注册账号。

　　认证登录后，创建第一个库(repository)：

![创建repository1](http://i1.tietuku.com/b369ad5478529d59.png)
![创建repositoty2](http://i1.tietuku.com/242be3da7863423e.png)

　　在1处输入库的名字，一定要按照这个格式username.github.io，此处username是你自己

的昵称。2是你对该库的一个描述，最后点击3就行了。

　　接下来我们需要在新建的rep中添加一个CNAME文件，这个文件github用来把域名转换为IP地址

的。

![创建CNAME1](http://i1.tietuku.com/10704ac15fab3b56.png)

　　在CNAME文件中输入自己的域名：

![创建CNAME2](http://i1.tietuku.com/8276a7f2c3ec58f3.png)

**DNS解析服务:**

　　有了自己的域名和github后，现在需要把域名和github服务器绑定起来，意思就是当别人在

浏览器搜索栏键入你的域名之后，DNS服务器能够把域名解析到github相应的IP上从而访问到你

博客的页面，前面说域名就相当于你的名字，而一个IP地址就相当于你的身份证号。

　　我使用的DNS解析是[DNSPod](https://www.dnspod.cn),一样的注册登录，然后添加自己的域名：

![DNS解析域名1](http://i1.tietuku.com/ffcbace8a42b746c.png)
　　

　　首先添加域名，然后输入你的域名点击确定。

![DNS解析域名2](http://i1.tietuku.com/12162889def7d6cf.png)

　　进入添加的域名后，点击添加记录，一共添加三个记录，第一个记录类型为CNAME，记录值对应你

的rep名；第二个和第三个记录类型为A，记录值分别对应github服务器的两个IP。注意github的IP

会不时的变动，如果发现自己的网站出现解析问题很可能是github的IP更新了。

**总结**

　　OK,以上就是所有的准备工作，等待一段时间后键入你的域名发现能转入到github主页时那就说明

你成功了。


