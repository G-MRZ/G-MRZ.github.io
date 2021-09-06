---
title: "Vim插件"
date: 2021-07-31T23:56:54+08:00
draft: false
images: []
tags: [ "vim/neovim" ]
---

# 插件
1、vim-plug 插件管理器 [https://github.com/junegunn/vim-plug](https://github.com/junegunn/vim-plug)

2、coc-nvim 代码补全 [https://github.com/neoclide/coc.nvim](https://github.com/neoclide/coc.nvim)

3、nerdtree 目录树 [https://github.com/preservim/nerdtree](https://github.com/preservim/nerdtree)

## vim-plug
###### windows安装方法
```
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni $HOME/vimfiles/autoload/plug.vim -Force
```
###### Unix安装方法
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
###### vim配置文件添加
```
call plug#begin('~/.vim/plugged')
    Plug 'scrooloose/nerdtree', { 'on':  'NERDTreeToggle' }
call plug#end()

 /*
  ~/.vim/plugged为插件安装目录 
 */
```

### vim-plug常用命令

```:PlugInstall```安装插件

```:PlugUpdate```更新插件

```:PlugUpgrade```更新vim-plug

" NERD tree 插件会在首次使用 NERDTreeToggle 命令时进行加载

Plug 'scrooloose/nerdtree', { 'on': 'NERDTreeToggle' }

" 多个命令

Plug 'junegunn/vim-github-dashboard', { 'on': ['GHDashboard', 'GHActivity'] }

" 当文件类型为 clojure 时，加载插件

Plug 'tpope/vim-fireplace', { 'for': 'clojure' }

" 多种文件类型

Plug 'kovisoft/paredit', { 'for': ['clojure', 'scheme'] }

" 当首次执行 Vader 命令，且文件类型为 vader 时，加载插件

Plug 'junegunn/vader.vim',  { 'on': 'Vader', 'for': 'vader' }

" 插件按需加载后执行特定代码

Plug 'junegunn/goyo.vim', { 'for': 'markdown' }

autocmd! User goyo.vim echom 'Goyo is now loaded!'

## coc-nvim
###### 安装
```
call plug#begin('~/.vim/plugged')
    ***
    Plug 'neoclide/coc.nvim', {'branch': 'release'}
call plug#end()
```

### coc-nvim常用命令

```:CocInstall [插件名称]```安装插件

```:CocUninstall [插件名称]```卸载插件

```:CocList extensions```打开安装插件列表

```:CocConfig```打开用户配置 ```coc-settings.json```

```:CocLocalConfig```打开项目配置文件

```:checkhealth```检查 NeoVim 状态

```:CocInfo```查看 coc.nvim 服务相关信息

```:CocRestart```重启 coc 服务





