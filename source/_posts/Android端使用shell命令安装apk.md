---
title: Android端使用shell命令安装apk
date: 2024-01-03 23:46:53
tags: 其他
cover: https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-01-03%20234819.png
---

安卓端进行 shell 命令静默安装时会报错：

Cannot run program “pm “: error=13, Permission denied

解决方法：

将文件拷贝到/data/local/tmp/下再进行安装

![Screenshot_2025-02-12-17-05-45-892_com.jozein.xedgepro](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedScreenshot_2025-02-12-17-05-45-892_com.jozein.xedgepro.jpg)![A5C1AA86B9B08F1790BD7CEFB861571A](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedA5C1AA86B9B08F1790BD7CEFB861571A.jpg)
