# 项目部署

> 
## 项目介绍
> 此项目基于小程序 ▪ 云开发，不用搭建后台，首页字体和其他页面的图标都是在线的，字体用的是 iconfont 在线字体（站酷小薇体），[字体地址](https://www.iconfont.cn/webfont?spm=a313x.7781069.1998910419.d81ec59f2#!/webfont/index "字体地址")。
> 项目共有4个页面，分别是index首页，album相册列表页，picture图片列表页，create创建相册页。
> 如需下载部署，请按照下面步骤，导入项目。

## 步骤一 导入项目
注册小程序（如果不会注册小程序请自行百度），创建项目时选择云开发。、

## 步骤二 创建数据库
打开云开发控制台
1. 首先添加welcome集合，权限设置为=>所有用户可读，仅创建者可读写，然后添加一条随机记录，字段名为=>image_url，类型为=>string，值为图片的url地址。
2. 添加album集合，权限设置为=>所有用户可读，仅创建者可读写。
3. 添加picture集合，权限设置为=>所有用户可读，仅创建者可读写。

## 步骤三 编译项目
上面的步骤都部署好之后就可以运行项目了。

## 注意事项
上传图片时需要验证用户的openid，进入图片列表页，打开调试窗口AppData，找到你的openid复制，在picture.js下面，找到如下代码，替换为你的openid即可。

`if (this.data.openid !== '你的openid')`

## 项目体验
微信扫描下面二维码即可体验。
![](https://github.com/15113624649/mini_album_project/blob/master/miniprogram/mini_album.jpg)

