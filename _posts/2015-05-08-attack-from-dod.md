---
layout: post
title: "attack from DOD"
description: ""
category: 
tags: []
---
{% include JB/setup %}

昨晚看到服务器上log不大对，怎么有那么多的404错误呢。一波三折啊，搞不懂支付公司的烂网络了。

在log里看到很多访问，问题有：

1. 所有的web访问来源都是同一个IP
2. IP地址来源是美国？怀疑是堡垒机VPN搞的
3. 访问的POST数据中有很多没有201错误，没有绑定小票机。

todo
    vpn环境下检查traceroute到堡垒机和服务器上抓到的访问机器的IP
    和支付公司确认IP来源，和小票机访问账号的问题（配置、权限等）
    对log分析的命令进行整理

