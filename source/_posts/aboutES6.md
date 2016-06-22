---
title: ES6的一些心得
date: 2016-06-22 10:18:21
tags: web前端
categories: web前端
description: 最近在写一些chrome扩展，这个纯粹的chrome运行环境比较适合拿es6的一些新特性来练手。记下一些对es6的使用心得体会。
---

最近在写一些chrome扩展( [github repo](https://github.com/unclehking?tab=repositories) )，这个纯粹的chrome运行环境比较适合拿es6的一些新特性来练手。记下一些对es6的使用心得体会。

**1、字符串模板**
前端编程有很大部分情况是在“拼接字符串”，这是个非常糟糕的编程体验。
以前:
``` bash
var str = //
var html =  "<ul><li>"+str+"<li><ul>";
```
ES6:
``` bash
var str = //
var html =  `<ul>
		<li>${str}</li>
	    <ul>`;
```
使用字符串模板和反引号，使的字符串可以换行，拼接html结构字符串的时候能保清晰的格式，直观便捷。(字符串模板只反引号中使用才有效，"abc${str}123"就只是个普通的字符串了。)
