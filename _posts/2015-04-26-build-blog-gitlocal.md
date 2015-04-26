---
layout: post
title: "手把手教你用Github搭建独立博客（三）"
date: 2015-04-26 9:32:00
categories: blog-build
featured_image: /images/cover.jpg
---
##Github Local

　　本讲主要介绍一下如何建立本地repo并和github服务器（以下统一称作远端）上的

repo进行同步，涉及到的文件结构属于jekyll部分内容，下一讲会详细提到。

　　First，我们需要下载github的命令窗口程序——[Git Bash](http://git-scm.com/download/)，咱们到时候把本地修改

提交到远端和同步远端的修改都要使用到git command。

　　下载完成之后，在本地你喜欢的地方建立一个文件夹，命名为username.github.io

（username还是你github的用户名），然后在文件夹里建立如下图所示的文件结构：

![本地文件结构](http://i1.tietuku.com/ed78f8e4ec78e965.png)

　　
PS:这些文件具体是做什么的下一讲会进行详细介绍。

　　在根目录下index.html文件中添加内容：

    {% highlight html %}
      <html>
		<head>
			<title>My Blog</title>
		</head>
		<body>
			<p>Hello World!</p>
		</body>
	</html>
	{% endhighlight %}
　　

　　在文件根目录下点击鼠标右键运行git bash，输入如下命令：
    
     git init                             
     #初始化本地库
     git add -A
     #添加该文件到本地库
     git commit -m "files"
     #确认提交
     git remote add origin https://github.com/username/username.github.io.git
     #添加远端在本地引用	
     git push origin master
     #提交修改



　　

　　如果想要全面学习git命令，请戳右边——>[Git命令大全](http://www.yiibai.com/git/home.html)

　　OK，现在登录github，可以看到上面也有和本地一样的文件结构啦~：

![远端文件结构](http://i1.tietuku.com/8433df91974c8f6e.png)

　　浏览器键入你的域名后应该就可以看到自己的Hello World首页了：

![hw_index](http://i1.tietuku.com/33eb41b39554d3c5.png)