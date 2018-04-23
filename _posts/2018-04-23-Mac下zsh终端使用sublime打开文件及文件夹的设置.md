---
layout: post
title: Mac下zsh终端使用sublime打开文件及文件夹的设置
categories: [Mac]
tags: Mac sublime
---

## Mac下zsh终端使用sublime打开文件及文件夹的设置

<!--# 简介
Mac下zsh终端使用sublime打开文件及文件夹的设置-->

## zsh设置
- 编辑zsh配置文件
```bash
$ vi ~/.zshrc
```

- 添加如下配置内容
```text
alias subl="open -a 'Sublime Text'"
```

- 保存退出，使zsh配置生效
```bash
$ source ~/.zshrc
```

## 原理浅析
```text
利用了命令"open -a 'Sublime Text' /home/Documents/xxx"
```

## 参考
- (如何在mac中用命令行时用sublime打开文件)[https://segmentfault.com/q/1010000002397241]









