---
title: 原神官服B服切换方法
date: 2023-01-30 16:38:45
tags: 其他
cover: https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20170144.png
---

原神官服 B 服切换方法

众所周知，原神官服 b 服不互通，这给有两个服的账号的玩家带来很多麻烦。解决方法有很多，可以分别下载官服与 b 服【这种方法不仅占用磁盘空间，而且会出现吞服的情况（后面会给出解释）】，也可以自行更改配置文件（这种方法比较麻烦，每次换服时都要更改配置文件，官服还会让重新输入账号密码）。

本人作为一名提瓦特人，深受其扰。

偶然的机会，我刷到 b 站的一个视频，灵感大发。我参考了这个视频[轻松自制原神双服转换器*哔哩哔哩 bilibili*原神](https://www.bilibili.com/video/BV1mW4y117wo/?spm_id_from=333.999.top_right_bar_window_history.content.click&vd_source=0875a89ce3e551ffadbd073e593b6329)，并在此基础上进行了优化。

# 一、电脑上现有官服原神（以官服为基础改造）

## Ⅰ.傻瓜教程

图片的上方边缘部分有路径地址，方便参考

1.下载 链接:https://www.123912.com/s/23C1jv-oiCzH?pwd=chou# 提取码:chou并解压其中的zip文件

2.在桌面上找到原神启动器，右键单击，点击“打开文件所在的位置”

![屏幕截图 2023-01-30 162904](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20162904.png)

3.点开“Genshin Impact Game”文件夹

![屏幕截图 2023-01-30 163003](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20163003.png)

4.将第 1 步下载的文件夹中的这三个文件放入“Genshin Impact Game”文件夹中

![屏幕截图 2023-01-30 163112](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20163112.png)

5.点击“YuanShen_Data”文件夹

![屏幕截图 2023-01-30 163135](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20163135.png)

6.点击“Plugins”文件夹

![屏幕截图 2023-01-30 163158](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20163158.png)

7.将第 1 步下载的文件夹中的这两个文件放入“Plugins”文件夹中

![image-20250730124311263](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/image-20250730124311263.png)

8.将“Genshin Impact Game”文件夹下的这三个文件快捷方式发送到桌面

![屏幕截图 2023-01-30 180855](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20180855.png)

9.在桌面上双击对应的文件即可启动对应服务器

![屏幕截图 2023-01-30 170144](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20170144.png)

## Ⅱ.原理

1.本程序是运用批处理实现的

2.代码解释

bat 批处理文件原理
使用“ren”命令对文件进行重命名，不会对游戏其他文件产生影响，右键文件编辑可查看和修改
例：ren（空格）源文件名（空格）改后文件名

![屏幕截图 2023-01-30 162735](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20162735.png)

![屏幕截图 2023-01-30 162800](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20162800.png)

config.ini.b 文件中存放的是 b 服所需配置文件，而 Genshin Impact Game 文件夹中的 config.ini 的初始文件中存放的是官服所需配置文件，游戏需要读取名为 config.ini 的文件中的内容。

以 b 服启动器为例，启动器将 config.ini 文件改名为 config.ini.g，将 config.ini.b 文件改名为 config.ini，

由此把官服的配置文件改为 b 服的配置文件，游戏会读取到 config.ini 中的 b 服配置信息，从而打开 b 服渠道。

官服启动器原理亦是如此。

有旅行者可能要问了，连续点击两次同一个服务器的启动器，config.ini.b 或者是 config.ini.g 的文件内容岂不是要发生变化？

下面这张图片将会为你解开迷惑

![屏幕截图 2023-01-30 161151](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-30%20161151.png)

批处理时，如果存在与要输出的文件的文件名相同的文件，程序将不执行/跳过该命令（上图的第一个指令）；

如果找不到目标文件，程序也将不执行/跳过该命令（上图的第二个指令）。

从而无事发生，继续执行第三个指令：启动游戏。

由此可见，官服和 b 服用了同一个游戏本体，却通过 config.ini 文件来分配渠道，因此当两个游戏本体放在一起时会出现吞服的情况。

# 二、电脑上现有 b 服原神（以 b 服为基础改造）

本人太懒，没有实操以 b 服为基础改造的情况，请各位旅行者参考这位 b 站大佬的教程

[原神 PC 端 B 服官服一键切换方法 - 哔哩哔哩 (bilibili.com)](https://www.bilibili.com/read/cv14893226?spm_id_from=333.999.0.0)

（这位大佬有教如何改变 bat 文件的图标哦）

我把图标放在下面了

![QQ图片20230130170044](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedQQ%E5%9B%BE%E7%89%8720230130170044.jpg)

![QQ图片20230130164306](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedQQ%E5%9B%BE%E7%89%8720230130164306.jpg)

![img](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedzjhimgbedzjhimgbedf77dbb45e7ab9ea2052528b7379622eb52786664.png@100w_100h.ico)

教程完。
