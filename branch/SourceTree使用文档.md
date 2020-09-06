# SourceTree使用文档

@[SourceTree]

[TOC]

## Git下载及安装

>Git是一个开源的分布式版本控制系统，可以有效、高速的处理从很小到非常大的项目版本管理。Git 是 Linus Torvalds 为了帮助管理 Linux 内核开发而开发的一个开放源码的版本控制软件。

[Git下载地址](https://git-scm.com/downloads)
Git安装教程参考：[安装Git教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00137396287703354d8c6c01c904c7d9ff056ae23da865a000)

## SourceTree下载及安装

> **SourceTree** 是 Windows 和Mac OS X 下免费的 Git 和 Hg 客户端管理工具，同时也是Mercurial和Subversion版本控制系统工具。支持创建、克隆、提交、push、pull 和合并等操作。

SourceTree下载地址：https://www.sourcetreeapp.com/ 或者 https://www.sourcetreeapp.com/download-archives

**Windows**系统用户安装过程中**（暂无Mac解决方法，Mac用户请按照安装步骤操作）**，会遇到授权登录Atlassian操作，如果没有Atlassian账号没有翻墙的话，不容易通过该步骤，如下图：
![@图2-1](https://images2017.cnblogs.com/blog/1135985/201801/1135985-20180104130310737-2100428098.png)
<br/>

请按照[sourcetree跳过注册的方法](https://www.cnblogs.com/lucio110/p/8192792.html)操作，完成安装。
请按照[sourcetree跳过注册的方法](https://blog.csdn.net/weixin_41394654/article/details/104726290)操作，完成安装。

## SourceTree使用方法

###Clone项目

进入SourceTree主页，将Gitlab上的项目Clone下来
<br/>
![@图3-1](./1523327988975.png)
<br/>


**例如：**
将datacube-athena项目clone：
<br/>
![@图3-2](./1523328203843.png)
<br/>

clone后如图：
<br/>
![@图3-3](./1523328418487.png)
<br/>

检出dev分支：
<br/>
![@图3-4](./1523328666587.png)
<br/>


###拉取分支
分支管理流程及使用规范：http://192.168.8.215:8090/pages/viewpage.action?pageId=2785368

假如用户要在dev分支拉一个feature分支，操作如下图所示：
>**注意：**每次拉分支前，要首先拉取该分支下最新代码！

>![@图3-5](./1523329540449.png)

![@图3-6](./1523328939324.png)
<br/>

>**注意：**要定期拉取代码，确保你的代码是最新的。

###提交commit
![@图3-7](./1523329961716.png)

###提交merge request

登录Gitlab账号，点击头部tab页中的Merge Request，然后点击绿色的按钮"New Merge Request"，发起合并请求。

首先选择需要merge的分支以及将要合并到哪个分支：
<br/>
![@图3-8](./1523330319146.png)
<br/>
然后填写该分支修改描述：
<br/>
![@图3-9](./1523330494421.png)
<br/>
提交merge request成功后浏览file changes，确认修改的东西：
<br/>
![@图3-10](./1523333060865.png)


###删除本地分支

右键分支，选择删除分支（不可选择**dev**和**master**分支），弹框中勾选"强制删除"，完成删除本地分支操作。
>**注意：**在保证你的分支以及被合并到dev或者master后，确保你的分支已经没有用了，再执行删除操作。