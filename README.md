# IQuickLook
IQuickLook-Mac快速预览工具。不用打开文件就能看到文件中的内容或信息!

@[TOC](MacOS效率工具IQuickLook-多合一Quick Look快速预览与右键扩展信息工具)
# 系统说明
系统：macOS 10.15或以上

# Quick Look说明
## 什么是Quick Look
Quick Look 是 Mac上超方便的功能，用户可以在不打开外部软件的情况下按下空格键快速预览文件。

对于常见文件，例如jpg、png、gif等图片格式，doc、txt、ppt等文档格式，sketch、ps、ai等设计师常用的源文件格式，都可以直接空格键实现即时预览，而不像 Windows 系统要双击打开应用后才能查看。在平时繁忙的工作中，这个功能无疑极大地提升了我们的工作效率。

## Quick Look的局限
Quick Look 目前的局限是系统能识别的文件格式预览的结果过于简单，很多时候不能满足用户的需求。这时就要安装quicklook插件来补充这些功能。而QuickLook的插件很多，每个的功能比较单一。需要安装很多个插件。而且macOS 10.15之后苹果删除了一些旧的API。新的API不允许QuickLook插件修改一些常用格式的预览界面。例如。png 、jpg、gif 等文件，从而导致了一些插件已经不能在新系统中使用

# “IQuickLook”应用程序的功能介绍
知道了Quick Look的目前的问题后。我们开发了一个名为“IQuickLook” 的macOS应用来扩展原来的功能同时解决现在这些问题。也就是说只要安装一个应用就能实现 QLImageSize、QLMarkdown、QLColorCode、QuickLookJSON等多个插件的功能。

本应用主要实现两个功能。功能一：Quick Look插件扩展支持更多文件格式；功能二:右键显示图片、音频、视频信息

## 功能一:Quick Look插件扩展支持更多文件格式
- 源代码高亮(.cpp .c .h .c# .php .java .js .py .swift .css .vue .yml .dart .sh .go 等)
- Markdown(.md .markdown .mdown .mkdn .mkd .rmd 等)
- 压缩文件(.tar .tar.gz .zip)
- 数据交换文件(.json)
- 数据库脚本(.sql )
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201101151951395.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3N1Z29vZHM=,size_16,color_FFFFFF,t_70#pic_center)
实际上我们这个工具支持的格式远不止上面例举的，以后还会支持更多的语言

## 功能二:右键显示图片、音频、视频信息
*由于一些图片、音频、视频文件在新版macOS中使用Quick Look插件已经无法自定义界面。所以我们通过扩展Finder（访达）的右键功能来显示图片、音频、视频的信息。*

图片支持格式(.jpg .png .gif .psd .bmp .tif .svg 等)
视频支持格式(.mp4 .3gp )
音频支持格式(.mp3)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201101154730522.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3N1Z29vZHM=,size_16,color_FFFFFF,t_70#pic_center)
# “IQuickLook”应用程序安装
## 下载文件
- [IQuickLook安装包下载](https://github.com/sugood/IQuickLook/releases)
- App Store 下载（正在审核中）

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201101161450610.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3N1Z29vZHM=,size_16,color_FFFFFF,t_70#pic_center)
## 安装完成后需要打开两个扩展权限
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201101161752340.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3N1Z29vZHM=,size_16,color_FFFFFF,t_70#pic_center)
## 设置Finder扩展的执行路径
*一般设置为根目录（ / ）即可。如果文件不在设置的目录下，右键无法显示文件信息*
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201101162044869.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3N1Z29vZHM=,size_16,color_FFFFFF,t_70#pic_center)

# 注意事项
1. 右键显示图片、音频、视频信息功能目前只支持本地SSD。扩展硬盘或者外接硬盘暂不支持
2. 由于最近才完成应用开发，所以，可能会存在一些BUG。希望大家多多包涵。有任何问题都可以留言或者提交到我们[github](https://github.com/sugood/IQuickLook)的[issues](https://github.com/sugood/IQuickLook/issues)中。
