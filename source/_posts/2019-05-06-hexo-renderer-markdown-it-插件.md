---
title: hexo-renderer-markdown-it 插件
tags: [Hexo,插件,Markdown, markdown-it]
date: 2019-05-06 17:07:31
categories: Hexo
---

## Hexo插件hexo-renderer-markdown-it使用
### 简介
`hexo-renderer-markdown-it`是一款用于Markdown解析和渲染的插件,用于替换Hexo默认自带的Markdown解析器，其对github format markdown 和标准的commonmark支持比较好，而且有丰富的markdown-it插件，可以丰富markdown的渲染

### 安装
1. 先卸载Hexo默认自带的Markdown渲染器

        npm uninstall hexo-renderer-marked --save
2. 安装hexo-renderer-markdown-it 插件

       npm i hexo-renderer-markdown-it --save

### 配置
在Hexo的主配置文件`_config.yml`中进行配置，配置分两种方式：
- 简单配置 (支持三种配置级别，zero, default, commonmark)
- 高级配置（用户自定义，渲染器，插件等）  
- 在Hexo的_config.yml配置文件中添加如下字段

        # markdown-it config
        markdown: 'commonmark'

### markdown-it 插件
markdown-it的插件可以增强他的解析功能，可访问此[插件列表](https://www.npmjs.com/search?q=keywords:markdown-it-plugin)搜索所有可用的markdown-it插件

### markdown-it 在线语法学习
这里有一个在线的markdown-it语法学习环境[markdown-it](https://markdown-it.github.io/)

参考资料：
- [Markdown-it](https://github.com/markdown-it)
- [Markdown-it插件详解](https://www.jianshu.com/p/588ab3d22eb8)