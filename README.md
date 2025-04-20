<!-- @format -->

# 我的个人博客

这是使用 Jekyll 和 GitHub Pages 搭建的个人博客。

## 本地开发

### 环境要求

-   Ruby 2.5.0 或更高版本
-   RubyGems
-   GCC 和 Make（用于安装本地扩展的 gem）

### 安装步骤

1. 安装依赖：

```
bundle install
```

2. 本地预览：

```
bundle exec jekyll serve
```

3. 在浏览器中访问：

```
http://localhost:4000
```

## 部署

该博客将自动部署到 GitHub Pages。当您将更改推送到仓库的 main 分支时，GitHub 会自动构建和发布网站。

## 创建新文章

在`_posts`目录下创建新的 Markdown 文件，文件名格式为`YYYY-MM-DD-title.md`。
文件开头需要包含 YAML 头信息：

```yaml
---
layout: post
title: "文章标题"
date: YYYY-MM-DD HH:MM:SS +0800
categories: blog
---
```
