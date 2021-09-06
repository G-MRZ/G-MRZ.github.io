---
title: "Nvm"
date: 2021-08-15T22:56:32+08:00
draft: false
images: []
tags: [ "nvm" ]
---

# 安装

```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
```
## 常用命令
```nvm install [version number]``` 安装固定版本node

```nvm uninstall [version number]``` 卸载固定版本node

```nvm ls``` 列出已安装node

```nvm use [version number]``` 切换版本

```nvm ls-remote``` (linux)查看远程服务器所以可用版本
```nvm ls available``` (windows)查看远程服务器所以可用版本

