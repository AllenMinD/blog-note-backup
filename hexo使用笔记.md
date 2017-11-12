---
title: Hexo使用笔记
date: 2017/9/17 13:05:00
categories:
- 学习
tags: 
- Hexo
- 博客搭建
---
这是文章摘要:这篇文章主要写了Hexo常见使用方法。
<!--more-->

<h1>Hexo使用笔记</h1>

[官方文档](https://hexo.io/zh-cn/docs/)

<h3>1. 创建hexo（初始化hexo）</h3>

	//安装 Hexo 完成后，请执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。
	hexo init 文件名
	cd 文件名
	npm install

<h3>2. 配置文件_config.yml中各项的含义</h3>
看[这里](https://hexo.io/zh-cn/docs/configuration.html)
<h3>3. 常用指令</h3>

	hexo n #写文章
	hexo g #生成
	hexo d #部署到服务器 #可与hexo g合并为 hexo g -d
	hexo clean #清除缓存文件 (db.json) 和已生成的静态文件 (public)。在某些情况（尤其是更换主题后），如果发现您对站点的更改无论如何也不生效，您可能需要运行该命令。
	hexo s #启用本地服务器，用来进行本地预览

[其他指令](https://segmentfault.com/a/1190000002632530)

<h3>4. Front-Matter</h3>
Front-matter 是文章最上方以 `---` 分隔的区域，用于指定个别文章的变量。具体看[这里](https://hexo.io/zh-cn/docs/front-matter.html)。
<h3>5. 文章摘要</h3>
和WordPress一样，Hexo创建文章摘要要使用`<!--more-->`。  
	
	//文章摘要一般放在每篇文章文件的Front-Matter下面，这样的话，在more之上，Front-Matter之下的内容就是显示出来的文章摘要
	
	摘要内容
	<!--more-->

