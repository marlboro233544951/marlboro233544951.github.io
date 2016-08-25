---
layout: post
title: 蛋疼的社会化评论插件
date: 2016-8-20
categories: blog
tags: [网页前端]
description: 多说评论的使用
---

# 兜兜转转一整天还是用了多说

瞎折腾了一天，去选择各种评论插件或者自己手写插件，最后还是选择了多说。

先谈谈自己尝试使用的插件吧。

1.  畅言
	属于搜狐的第三方社会化插件，个人觉得搜狐能够为这款插件的隐私保护背书，但是这款插件的使用需要国内的IPC备案，由于我的域名和服务器都在国外，所以没有拥有使用畅言的完整权限，故放弃了。

2. 	echo-chamber-js
	github上的一个项目[echo-chamber-js](https://github.com/tessalt/echo-chamber-js)，这是一个将评论保存在浏览器的local storage中的插件，只能本地同一个浏览器浏览，显然不是我需要的

3.  Comm\(ent\|it\)

	>This repository contains the code of the application hosted at commentit.io. Comm\(ent\|it\) uses the Github API and Jekyll to help storing visitors comments directly in Github Pages repository. You can contribute to make it better and more reliable.

	这个插件其实是我的第二选择，因为不太想折腾了，所以没有选择使用。这个插件完全契合这个博客的搭建方式，只是评论需要github账户，这点对于大多数人来说并没有github的账户，但是这未必不是一个筛选交流人群的方式。

4.  多说
	图方便吧，设置方式很简单，代码段贴进来，对应多说账户设置好，就能够用了，但是所有的评论是保存在多说的服务器上的，个人感觉很蛋疼。因为信息存储不是在自家能控制的范围。

5.  手写插件
	个人觉得还是没精力去学习做一个插件，暂时没有想学习服务器端知识的打算，就放弃了。