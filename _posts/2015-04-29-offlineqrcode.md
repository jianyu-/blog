---
layout: post
title: "offlineQrcode"
description: "离线条码开发"
category: develop
tags: [二维码、支付宝]
---
{% include JB/setup %}


####开始准备动手干**离线条码**。

问题包括：

1. 如何定义一个容易分发的django模块，需要注意的点有哪些
2. 缺少android和iOS的实现，FPE部分
3. 二维码中间嵌入图片的实现方式还不清晰
4. 性能测试方法，是否采用nginx＋django？

### 如何开发可以复用的django模块


    .
    |-- _config.yml
    |-- _includes
    |-- _layouts
    |   |-- default.html
    |   |-- post.html
    |-- _posts
    |   |-- 2011-10-25-open-source-is-good.markdown
    |   |-- 2011-04-26-hello-world.markdown
    |-- _site
    |-- index.html
    |-- assets
        |-- css
            |-- style.css
        |-- javascripts

### PIL如何操作QRCode
    QRCode生成的PNG格式图片，根据内容大小不同，图片大小也不同
