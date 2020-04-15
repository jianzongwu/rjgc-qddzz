# 调研报告

PB17111634 刘文勋

## 选型

微信小游戏：圈地大作战

## 实现功能

可以通过微信登录和好友一起玩游戏

（可以以微信上的游戏作为参考进行开发）

## 小程序结构

根据微信小程序的开发文档，小程序的结构包括：

**框架，组件，api和服务端api**

**组件**包括：视图容器，基础内容，表单组件，导航，媒体组件，地图，画布，开放能力，原生组件，无障碍访问导航栏和页面属性配置节点

**api**包括：基础api，系统api，小程序api，界面api，网络api，媒体api，开放接口api

**服务端api**包括：登录api，用户信息api，接口调用凭证api，数据分析api，访问留存api，访问趋势api，客服消息api，模板消息api，统一服务信息api，动态消息api，插件管理api，附近的小程序api，小程序码api，内容安全api，即时配送api，物流助手api，

## 开发工具

egret wing <:http://developer.egret.com/cn/github/egret-docs/Wing/update/update320/index.html>

labrator:<https://github.com/maichong/labrador>

通过查阅，我倾向于使用egret wing开发，原因有三：1.文档详实，2.自带IDE，3.可实时预览

![img](http://cdn.dev.egret.com/egret-docs/Wing/update/update320/1.png)

![img](http://cdn.dev.egret.com/egret-docs/Wing/update/update320/7.gif)

![img](http://cdn.dev.egret.com/egret-docs/Wing/update/update320/4.gif)

![img](http://cdn.dev.egret.com/egret-docs/Wing/update/update320/5.gif)

![img](http://cdn.dev.egret.com/egret-docs/Wing/update/update320/8.gif)

看起来使用效果相当不错

对于代码补全也许可以再加上一些插件，比如sublime或vscode

## 开发教程

第一弹：<http://www.diycode.cc/topics/311>

第二弹：<http://www.diycode.cc/topics/312>

第三弹：<http://www.diycode.cc/topics/316>

第四弹：<http://www.diycode.cc/topics/325>

第五弹：<http://www.diycode.cc/topics/328>

从这五个教程来看似乎并不需要自己的服务器加持，仅仅是在官方给的网站上进行代码块的加载生成的程序，查看了一些小程序的代码:<https://github.com/litt1e-p/weapp-girls>（包括server端的代码，我认为是腾讯所提供的服务器），似乎确实如此。

但是也在网上看到可以用Matchvs作为游戏云。这个部分在具体实操时再进行考虑。

## 环境

win10

wechat_devtools+javascript

node.js

egret

github

也许会用到matchvs