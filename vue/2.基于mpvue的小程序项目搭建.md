#基于mpvue的小程序项目搭建

###初始化

第一步

```
$ npm install --global vue-cli@2.9.6
```
第二步
```
$ vue init mpvue/mpvue-quickstart my-project
```
第三步
```
$ cd my-project
$ npm install
$ npm run dev
```

###微信开发者工具

下载地址：https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html

###调试开发

appID在这里：
![enter image description here](https://img-blog.csdn.net/20180129232806273?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvTEpGUEhQ/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

打开微信开发者工具，然后：

![enter image description here](https://upload-images.jianshu.io/upload_images/5640239-736f301592d265d6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/826/format/webp)

![enter image description here](https://upload-images.jianshu.io/upload_images/5640239-4bad54b5b33b140d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/418/format/webp)

###真机调试及上传

真机调试：写完代码，点“真机调试”按钮，然后扫码就能看了。

上传：在要发布代码之前，要把代码上传到微信公众平台，上传后可以在微信公众平台的“开发管理”中看到![Alt text](./CB376BED-9DA8-4dec-8CB8-E7EE7219BA0C.png)
可以发布体验版供他人浏览，但事先要在“用户管理”添加
![Alt text](./CD5272B6-0C86-462f-ABE9-7CC093AC961F.png)

