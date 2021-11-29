---
title: "Neovim"
date: 2021-08-08T15:02:23+08:00
draft: false
tags: ["工具"]
---

### 安装

```html
 ### windows
下载[nvim-win64.zip](https://github.com/neovim/neovim/releases), 解压到本地目录（自己选), 在解压后文件中找到bin目录， 复制其绝对路径添加到Windows用户环境变量
 ~/AppData/Local/nvim/init.vim  <!--windows配置文件路径-->

### linux
sudo apt install neovim
~.config/nvim/init.vim  <!--配置文件路径-->
```

### vim-plug安装

```Shell
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

### 命令

```Shell
:terminal # neovim中打开终端
```
