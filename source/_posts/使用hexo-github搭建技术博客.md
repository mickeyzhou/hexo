---
title: 使用hexo和github搭建博客
date: 2019-04-29 17:17:34
categories: Hexo
tags: Hexo
---
#### 1. 环境要求：
- 安装git
- 安装node

#### 2. hexo项目创建：
- 新建一个文件夹命名为blog, 并使用git init 命令将其初始化为一个本地仓库

- 使用npm install -g hexo-cli 安装hexo项目初始化脚手架工具

- 安装完后输入hexo -v 检查脚手架是否安装成
功

- 输入hexo init 生成hexo项目文件

- 项目文件生成后，输入hexo g 将markdown编译为静态文件

- 输入hexo s 启动本地博客web服务器，服务启动后在浏览器里输入<http://localhost:4000>就可以在本地预览编译生成的博客了

#### 3. 将本地的hexo项目部署到github
- 首先在个人的github上创建一个仓库，命名为blog， 创建时要勾选*initialize this repository with a README*

- 配置github与本地仓库通信用的密钥 ssh key

- 然后点击新建仓库的settings 向下拉到底部最后会有一个github Pages ， 选择一个主题，这个地址就是最终的博客访问地址

- 修改hexo项目的_config.yml配置文件，在文件最后一行有一个deploy配置，将其修改为
``` 
deploy:
  type: git
  repository: 这里填你在github上刚新建的仓库地址
  branch: master
```
- 修改-config.yml URL 配置选项，将url设置为github page的地址，将root设置为仓库的目录
```
 url: https://xxx.github.io/blog/
 root: /blog/ 
```

- 在hexo项目根目录，使用npm install hexo-deployer-git --save  安装一个部署hexo到github的npm 包

- 最后输入hexo d 就可上传你的本地hexo的代码到github仓库

- 上传完后访问仓库的github page 地址就是你的博客了

#### 4. 参考资料
- [hexo 官网](https://hexo.io/zh-cn/)
- [超详细Hexo+Github博客搭建小白教程](https://godweiyang.com/2018/04/13/hexo-blog/)

