---
title: vscode配置
date: 2023-08-13 17:15:40
tags: vscode
cover: https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-08-13%20165925.png
---

本文用于记录 vscode 配置数据

# 1.基础配置

参照[【教程】VScode 中配置 C 语言/C++运行环境\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1Cu411y7vT/?spm_id_from=333.337.search-card.all.click&vd_source=0875a89ce3e551ffadbd073e593b6329)

# 2.插件配置

参照[【教程】vscode 优化体验篇（推荐设置 && 推荐插件）\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1Hd4y1o7CN/?spm_id_from=333.880.my_history.page.click&vd_source=0875a89ce3e551ffadbd073e593b6329)

# 3.插件优化

在 2 中的 Code Runner 插件在使用时会出现中文字符乱码、无法弹出外部终端的情况，解决方法如下：

## 1.在扩展栏中找到 Code Runner，点击齿轮标志，点击扩展设置

![屏幕截图 2023-08-13 194139](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-08-13%20194139.png)

## 2.在打开的页面中点击如下图所示的选项

![屏幕截图 2023-08-13 194347](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-08-13%20194347.png)

## 3.找到如下图所示的两行，将其替换为如图所示的语句。（图后附代码）

![屏幕截图 2023-08-13 194754](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-08-13%20194754.png)

```
"c": "cd $dir && gcc -fexec-charset=GBK $fileName -o $fileNameWithoutExt && start cmd \"/c ; $fileNameWithoutExt &pause\""
```

```
"cpp": "cd $dir && g++ -fexec-charset=GBK $fileName -o $fileNameWithoutExt && start cmd \"/c ; $fileNameWithoutExt &pause\""
```

## 4.完成
