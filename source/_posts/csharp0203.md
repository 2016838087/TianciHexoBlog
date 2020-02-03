---
title: WebAPI全局异常处理
date: 2020-02-03 21:21:21
categories: .NET #分类
tags: ['技术'] #标签
---
### 记录一下WebAPI的全局异常处理

<!-- more -->

### 通常接口出现一些小错误，页面会返回一堆看不懂的代码

### 这对于我们寻找错误并没有什么太大的帮助，反而看着很难受
![错误信息](errormsg.png "错误信息")

### 遇到这种情况我们可以写一个全局异常过滤器，接口报错直接跳到过滤器

### 首先新建一个ActionFilter类（随便命名），继承至ExceptionFilterAttribute

### 代码如下
![ActionFilter](code.png "ActionFilter")

### 然后在WebApiConfig类里面全局配置

![WebApiConfig](code2.png "WebApiConfig")

### 只要接口出现异常就会跳到这个地方，返回我们定义的信息

![返回信息](backmsg.png "返回信息")

### 可以看到，尽管接口已经抛出异常了，但是网页返回的信息依旧是我所定义的

### 错误信息可以打印到日志，避免接口信息泄露，具体打印日志下期再说

# 学业繁忙，告辞

![告辞](byebye.jpg "告辞")