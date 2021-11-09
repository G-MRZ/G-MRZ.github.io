---
title: "Wsl安装图形界面"
date: 2021-10-24T16:34:17+08:00
draft: false
tags: ['wsl']
images: []
---

## wsl命令

```
wslconfig /list(wsl -l) 列出安装的子系统列表
wslconfig /setdefault Ubuntu-20.04 配置默认子系统
wslconfig /u Ubuntu-20.04 注销子系统
```

##### 1,安装xorg

```sudo apt install xorg. xorg是xfce桌面环境基础依赖```

#### 2,安装xfce4

```sudo apt install xfce4```

#### 3,安装xrdp

```sudo apt install xrdp```

##### 配置xrdp端口、向xsession写入xfce4-session

```
sudo sed -i 's/port=3389/port=3390/g' /etc/xrdp/xrdp.ini
sudo echo xfce4-session >~/.xsession
```

windows中启动远程桌面连接xrdp服务器打开linux桌面环境

#### 配置中文包

```
sudo apt install language-pack-zh-hans language-pack-zh-hans-base
#打开/etc/defalut/locale添加
LANG=zh_CNUTF-8
LANGUAGE="zh_CN:zh"

```

#### xrdp命令

```sudo service xrdp restart 重启```

```sudo service xrdp start 启动```