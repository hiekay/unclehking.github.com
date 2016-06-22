
---
title: 关于heox静态博客
date: 2016-05-08 13:41:40
tags: heox
description: 快速、简洁且高效的博客框架。Node.js 所带来的超快生成速度，让上百个页面在几秒内瞬间完成渲染。只需一条指令即可部署到 GitHub Pages, Heroku 或其他网站。
categories: 随笔
---

hexo基于nodejs

安装hexo
``` bash
npm install -g hexo
```

``` bash
hexo g
hexo s
hexo new "HKing"
```

github page部署
_config.xml

``` bash
deploy:
	type: git
	repository: git@github.com:unclehking/unclehking.github.io.git
	branch: master

hexo d
```
