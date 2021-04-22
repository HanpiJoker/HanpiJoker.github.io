---
layout: post
author: "HanpiJoker"
title: "neovim 文件管理插件（Defx.vim）"
---
# Defx
Defx 是neovim 新一代的异步文件树插件，项目链接是在 [Shougo/defx.nvim](https://github.com/Shougo/defx.nvim)。

## 插件安装
```shell
Plug 'Shougo/defx.nvim', { 'do': ':UpdateRemotePlugins' }
```

## 图标显示
1. Defx 文件树支持图标显示，所以我们首先需要安装 Nerd-Font；
```
# Manjaro with yay as Example
yay install nerd-fonts-complete 
```

2. 安装defx-icons 插件
```shell
Plug 'kristijanhusak/defx-icons'
```

## 配置文件示例
> 当前插件的github主页并没有放出很多的配置细节，可能插件还处于开发阶段。所以配置文件
> 会有很多快捷键的设置。

完整的配置文件位于[defx.vim](https://github.com/HanpiJoker/Config_Bak/blob/master/nvim/config/defx.vim)

***PS：配置文件并非原创，只是自己忘记从哪里下载的了。如果遇到原版，请以原版作者的为准***

## 快捷键速记

| Key   | Mode | Action
| ----- |:----:| ------------------
| `;`+`fl` | Normal | Open file explorer (toggle)
| `;`+`fa` | Normal | Open file explorer and select current file
| **Within _Defx_ window** ||
| `h/j/k/l` | Normal | Movement, collapse/expand, open
| `]`+`g` | Normal | Next dirty git item
| `]`+`g` | Normal | Previous dirty git item
| `w` | Normal | Toggle window size
| `N` | Normal | Create new file or directory
| `yy` | Normal | Yank selected item to clipboard
| `st` | Normal | Open file in new tab
| `sv` | Normal | Open file in a horizontal split
| `sg` | Normal | Open file in a vertical split
| `\` | Normal | Jump to project root
| `gx` | Normal | Execute associated system application
| `gd` | Normal | Open git diff on selected file
| `gl` | Normal | Open terminal file explorer
| `gr` | Normal | Grep in selected directory
| `gf` | Normal | Find files in selected directory
