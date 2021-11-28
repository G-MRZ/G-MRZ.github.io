---
title: "Vim插件"
date: 2021-07-31T23:56:54+08:00
draft: false
images: []
tags: [ "工具" ]
---

##### 插件

```html
1、vim-plug 插件管理器 [https://github.com/junegunn/vim-plug](https://github.com/junegunn/vim-plug)
2、coc-nvim 代码补全 [https://github.com/neoclide/coc.nvim](https://github.com/neoclide/coc.nvim)
```

##### vim-plug linux安装方法

```Shell
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

##### vim配置文件添加

```Shell
call plug#begin('~/.vim/plugged')
    Plug 'scrooloose/nerdtree', { 'on':  'NERDTreeToggle' }
call plug#end()

 /*
  ~/.vim/plugged为插件安装目录 
 */
```

##### vim-plug常用命令

```vim
:PlugInstall " 安装插件
:PlugClean " 移除不在列表中的插件
:PlugUpdate " 更新插件
:PlugUpgrade " 更新vim-plug
```

###### coc-vim安装

```vim
call plug#begin('~/.vim/plugged')
    ***
    Plug 'neoclide/coc.nvim', {'branch': 'release'}
call plug#end()
```

##### coc-nvim常用命令

```vim
:CocInstall [插件名称] " 安装插件
:CocUninstall [插件名称] " 卸载插件
:CocList extensions " 打开安装插件列表
:CocConfig " 打开用户配置 
:CocLocalConfig " 打开项目配置文件
:checkhealth " 检查 NeoVim 状态
:CocInfo " 查看 coc.nvim 服务相关信息
:CocRestart " 重启 coc 服务
```
