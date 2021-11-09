---
title: "wsl下Debian环境搭建"
date: 2021-11-09T13:44:42+08:00
draft: false
images: []
tags: ["linux"]
---

### wsl下Debian安装

1、Microsoft Store直接下载安装

2、[https://docs.microsoft.com/en-us/windows/wsl/install-manual](https://docs.microsoft.com/en-us/windows/wsl/install-manual)下载.Appx或者.AppxBundle安装包。解压于任意目录并运行解压出来的debian.exe程序

### hugo安装

[https://github.com/gohugoio/hugo/releases](https://github.com/gohugoio/hugo/releases)下载hugo*.dep安装包

```在安装包存放目录使用sudo dpkg -i hugo*.dep进行安装```

### wget curl git安装

```sudo apt install wget curl git```

### nvm安装

```curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash```

```wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash```

[debian基本命令](/blog/debian基本命令)

[hugo基本使用方式](/blog/hugo)

[nvm基本使用方式](/blog/nvm)