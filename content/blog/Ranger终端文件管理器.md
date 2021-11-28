---
title: "Ranger终端文件管理器"
date: 2021-08-15T16:15:52+08:00
draft: false
tags: ["工具"]
---

### 安装

```Shell
1, git clone git@github.com:ranger/ranger.git(如克隆到~目录)
2, cd ranger
3, sudo make install
```

### 生成配置

```Shell
ranger --copy-config=all # 生成默认配置文件于~/.config/ranger
```

### 常用命令

```Shell
touch <文件名> #创建文件
mkdir <文件夹名称> #创建文件夹
```

