---
title: 使用hexo+github搭建技术博客
date: 2019-04-29 14:58:25
tags:
---
1. 首先在github上创建一个存放博客项目的仓库
2. 使用npm install -g hexo-cli 安装hexo项目初始化脚手架工具
3. 安装完后输入hexo -v 检查是脚手架是否安装成功
4. 输入hexo init 初始化博客项目文件
5. 输入hexo g 生成静态文件
6. 输入hexo s 开启博客服务， 在浏览器打开http://localhost:4000就可以访问生成的博客网站了
7. 将hexo 创建的博客项目与github仓库关联， 修改_config.yml文件最后一行的deploy配置
8.  使用hexo new post xxx 创建一篇新博客
9.  使用markdown编写完博客后，在根目录下输入hexo g 命令生成静态网页,然后使用hexo s 命令就可以预览刚创建的博客了
10.  将博客部署到github主页上



