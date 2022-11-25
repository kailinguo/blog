---
title: Hexo 环境搭建
date: 2022-11-11 13:36:18
categories:
- 环境搭建
tags:
- 必看
---

官网：https://hexo.io/docs/

中文文档：https://www.w3cschool.cn/hexodocument/wzjr1liz.html

环境依赖：node12       py2.7

环境搭建：

- npm config set prefix "D:\develop\nodejs\node_global"
- npm config set cache "D:\develop\nodejs\node_cache"
- npm config set python D:\develop\python2.7
- npm config set sass_binary_site=https://npm.taobao.org/mirrors/node-sass
- npm config set registry https://registry.npm.taobao.org
- npm cache clean -f
- npm install -g hexo-cli
- npm install

本地启动：

```shell
    hexo server
```

先生成密钥不然无法发布：

```shell
    ssh-keygen -t rsa -C your_email@xxx.com
```

编译然后发布：

- hexo g
- hexo d