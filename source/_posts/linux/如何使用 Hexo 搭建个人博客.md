---
title: 如何使用 Hexo 搭建个人博客
link: how-to-install-hexo
date: 2023-08-16 22:05:46
tags:
- linux
- hexo
categories:
- blog
keywords:
- linux
- hexo
---
## 如何使用 Hexo 搭建个人博客

![Hexo Logo](https://hexo.io/logo.png)

Hexo 是一个快速、简单且强大的静态博客框架，它基于 Node.js 构建，能够帮助您快速搭建个人博客并发布到 GitHub Pages 或其他静态托管平台。以下是使用 Hexo 搭建个人博客的步骤：

### 步骤 1：安装 Node.js 和 Git

在开始之前，确保您的计算机上已经安装了 Node.js 和 Git。您可以从官方网站下载并安装它们。

- [Node.js 官网](https://nodejs.org/)
- [Git 官网](https://git-scm.com/)

### 步骤 2：安装 Hexo

打开命令行界面（终端），运行以下命令来全局安装 Hexo：

```bash
npm install -g hexo-cli
```

### 步骤 3：创建新的 Hexo 博客

在命令行中，导航到您希望创建博客的目录，然后运行以下命令：

```bash
hexo init my-blog
cd my-blog
npm install
```

上述命令将创建一个名为 `my-blog` 的新 Hexo 博客，并安装所需的依赖。

### 步骤 4：编写博文

在博客根目录下执行以下命令来创建新的博文：

```bash
hexo new "My First Post"
```

这将在 `source/_posts` 目录下创建一个名为 `my-first-post.md` 的 Markdown 文件。您可以在这个文件中编写博文内容。

### 步骤 5：自定义主题（可选）

Hexo 支持许多主题，您可以根据自己的喜好选择并安装主题。安装主题的步骤会因主题而异，但通常可以在主题的文档中找到相关指导。

### 步骤 6：生成和发布博客

在博客根目录下运行以下命令来生成静态页面：

```bash
hexo generate
```

然后，运行以下命令来发布博客到您选择的静态托管平台。例如，如果您想将博客发布到 GitHub Pages，可以运行：

```bash
hexo deploy
```

### 步骤 7：访问您的博客

完成发布后，您可以在浏览器中访问您的博客，通常是通过以下链接：

```
http://your-username.github.io/my-blog
```

### 结论

使用 Hexo 搭建个人博客是一个相对简单的过程，它允许您轻松创建和管理博客内容。通过遵循上述步骤，您可以快速搭建一个漂亮的个人博客，并与读者分享您的知识和想法。

希望这个简要的指南能够帮助您开始使用 Hexo 搭建您的个人博客！
