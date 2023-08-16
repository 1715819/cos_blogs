---
title: install python3.10 on linux
date: 2023-08-16 13:07:46
tags:
- linux
- python3
categories:
- linux
keywords:
- linux
- python3.10
---
## 如何在 Linux 编译安装 Python 3.10

![Python Logo](https://www.python.org/static/community_logos/python-logo-master-v3-TM-flattened.png)

Python 是一种广泛使用的高级编程语言，拥有丰富的库和工具，适用于各种应用场景。如果您在 Linux 系统上想要使用 Python 3.10，您可以按照以下步骤进行编译和安装。

### 步骤 1：准备工作

在开始之前，请确保您的 Linux 系统已经安装了必要的编译工具和依赖项。您可以使用包管理器来安装这些工具。在 Debian/Ubuntu 系统上，可以运行以下命令：

```bash
sudo apt update
sudo apt install build-essential libssl-dev zlib1g-dev libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev libffi-dev tk-dev
```

### 步骤 2：下载 Python 源码

前往 [Python 官方网站](https://www.python.org/downloads/source/) 下载 Python 3.10 的源码压缩包，并将其解压到您希望安装 Python 的目录中。

```bash
wget https://www.python.org/ftp/python/3.10.0/Python-3.10.0.tgz
tar -xzf Python-3.10.0.tgz
cd Python-3.10.0
```

### 步骤 3：配置编译选项

运行以下命令来配置编译选项。您可以根据自己的需求进行自定义配置。例如，您可以使用 `--prefix` 选项指定安装目录。

```bash
./configure --prefix=/usr/local/python3.10
```

### 步骤 4：编译和安装

使用 `make` 命令编译 Python 源码。

```bash
make
```

然后，使用以下命令进行安装：

```bash
sudo make install
```

### 步骤 5：验证安装

安装完成后，您可以使用以下命令验证 Python 3.10 是否正确安装：

```bash
/usr/local/python3.10/bin/python3.10 --version
```

您应该能够看到类似于以下的输出：

```
Python 3.10.0
```

### 结论

通过按照上述步骤，在 Linux 系统上成功编译和安装了 Python 3.10。现在您可以在您的系统中使用这个最新版本的 Python 来开发和运行您的应用程序。

请注意，编译安装 Python 可能会因系统配置和需求的不同而有所差异。在进行安装之前，务必仔细阅读 Python 官方文档以获取更多详细信息。

*文章分类：Linux*

希望这篇文章能够帮助您顺利在 Linux 系统上编译和安装 Python 3.10，让您能够充分利用这个强大的编程语言。