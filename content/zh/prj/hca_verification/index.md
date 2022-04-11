---
title: HCA验证平台
summary: 本工作对课题组开发的网卡作RTL级验证，使用UVM产生对网卡的输入激励并比对输出结果。
date: ""
publishDate: "2021-06-03T14:33:00+08:00"
lastmod: ""
#authors:
#- admin

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

comments: true
profile: true
share: false

gitment: true
slug: HCA-verification-cn

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""

categories:

tags:
- 验证
---

## **1. 函谷HCA介绍**
HCA是IB网络与主机之间的软硬件交互接口。我们的函谷HCA支持最多16K个QP和100Gbps的带宽。HCA卸载了地址转换和翻译功能，通过此功能网络数据可以旁路操作系统直接将数据写入内存。

## **2. 函谷HCA验证**
验证平台基于UVM搭建，整体结构图如下：

{{< figure src="framework.jpg" caption="Verification Framework" numbered="true" height="75%" width="75%" >}}