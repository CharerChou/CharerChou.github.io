---
title: win11美化
date: 2023-01-07 12:54:28
tags: win11
cover: https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedpreview.jpg
---

透明任务栏

在微软商店 Microsoft Store 下载 translucentTB

![屏幕截图 2023-01-07 131215](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-07%20131215.png)

![屏幕截图 2023-01-07 131305](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-07%20131305.png)

win11 开发版本更新后，任务栏透明工具 translucentTB 突然不管用了，在 b 站网友的指引下，我找到了 github 的开发者教程下的评论。

简单概括来如下：

# 法一：

## 1.下载 ViVeTool GUI

## 2.点击左上角的框，选择 25236![屏幕截图 2023-01-07 130135](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-07%20130135.png)

## 3.点击 Manually change a Feature (F12)，输入 26008830![屏幕截图 2023-01-07 130700](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-07%20130700.png)

## 4.点击右侧 Perforn Action ,点击 Deactivated Feature![屏幕截图 2023-01-07 130750](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-01-07%20130750.png)

## 5.关闭窗口，重启计算机。

—————————————————————————————————————————————

# 2023.4.24 更新

## 法一经测试在计算机重启后会失效，参考 b 站 up 的视频[Translucent TB 一键修复任务栏失效,无法透明\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1BT411Y7uc/?spm_id_from=333.1007.top_right_bar_window_history.content.click&vd_source=0875a89ce3e551ffadbd073e593b6329) 更新了使用 vivetool 的法二（法一是 vivetool GUI）

# 法二：

## 1.下载 vivetool[Releases · thebookisclosed/ViVe (github.com)](https://github.com/thebookisclosed/ViVe/releases/)并解压

## 2.用管理员身份运行 cmd

![屏幕截图 2023-04-24 083123](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-04-24%20083123.png)

## 3.在 cmd 中输入“cd ”（注意 cd 后有空格），再输入 vivetool 的文件位置，敲击 Enter

![屏幕截图 2023-04-24 083254](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-04-24%20083254.png)

## 4.输入“ .\ViVeTool.exe /disable /id:26008830 /variant:2”（注意最开始有空格和“.”）

![屏幕截图 2023-04-24 083448](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-04-24%20083448.png)

## 5.重启计算机

# 2023.6.30 更新

本次更新是因为傻卵微软今天的更新把法二也搞失效了。。。

# 法三：

## 1.下载 start11 链接：https://pan.baidu.com/s/18b6ZdecN18k_qCJ6Z1qkpg 提取码：chou 并安装

## 2.打开 start11，进入左侧的“任务栏”![屏幕截图 2023-06-30 103922](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-06-30%20103922.png)

## 3.点击“任务栏模糊、透明度及颜色”![屏幕截图 2023-06-30 104340](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-06-30%20104340.png)

## 4.点击“调节任务栏透明度”旁的“设置”，并调节不透明度为 0%![屏幕截图 2023-06-30 104457](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbed%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-06-30%20104457.png)

## 5.完成

# 2023.7.27 更新

更新了一些美化/实用工具

## 1.窗口最大化时任务栏自动隐藏，去除了透明任务栏带来的割裂感

链接：https://pan.baidu.com/s/1zlnZnIARw9WvVvdSaMB1Cw 提取码：chou

## 2.将某一窗口固定于屏幕上

链接：https://pan.baidu.com/s/1Q7XompuIZsRXvSfyRh9t_w 提取码：chou

# 2023.11.12 更新

win11 开始菜单“推荐的项目”无法彻底关闭，解决方法如下

## 1.下载下方文件

链接：https://pan.baidu.com/s/1qI5Lc7qAKkBiUwW08w_bOQ?pwd=chou
提取码：chou

## 2.把 ep_setup.exe 文件拖入 c 盘中的 Desktop

![image-20231112115238529](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedimage-20231112115238529.png)

## 3.右键单击“开始菜单推荐管理脚本.bat”，使用管理员权限运行，并按提示输入，回车即可

该文件运行完即可删除，无影响

脚本来源：

![image-20231112115735451](https://charerchou-imgbed.oss-cn-beijing.aliyuncs.com/CharerChou-imgBed/zjhimgbedimage-20231112115735451.png)
