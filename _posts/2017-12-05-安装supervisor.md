---
layout: post
title: 安装supervisor
categories: [code]
tags: Linux
---

# 安装supervisor

# 安装的时候要用yum install supervisor，
- 配置：vim /etc/supervisord.conf
- 启动：service supervisord start
- 管理：supervisorctl
*不要用pip install supervisor,这样不好加入系统服务，不便于启动supervisor服务，也不便于管理supervisor*

# 配置文件
/etc/supervisord.conf中添加如下：
``` conf
[include]
files = /etc/supervisord.d/*.ini

/etc/supervisord.d/文件夹下添加配置文件（config.ini）:
[program:ad_cms]
command=python Server.py
directory=/home/diyidan/ad
autorestart=true
stdout_logfile=/var/log/diyidan/ad.log
loglevel=info
```
