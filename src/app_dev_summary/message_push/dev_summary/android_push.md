# Android消息推送

## Android的离线推送

不同的品牌手机中的Android系统，有的还针对消息离线推送进行了特殊的定制，比如：

* 华为
* 小米

在系统级别上支持：app没有运行的情况下，也能收到离线消息。

所以总结Android端的离线消息推送，以及相关的应用保活：

> 注：应用保活=应用（在被系统杀掉后，仍然还能在后台运行）保（持）活（跃状态）

* 离线推送：
  * 优点：目前仅支持小米手机和华为手机，可以（借助小米／华为的androdi系统本身）实现app被杀掉仍能收到推送。
  * 缺点：覆盖度有限，其他机型没法支持
* 应用保活：
  * 优点：对于普通的用户的杀掉正在运行的app时，基本上可以实现app
  * 缺点：第三方管理软件理论上应该还是可以能把即使用了保活的app杀掉

-> 如果想要实现Android端的离线推送和应用保活的话，需要引导：

* 用户：把app加入系统和第三方管理软件的白名单
* 系统：用户自己把app加到系统的app白名单中，app进入后台后不会被杀掉
* 第三方管理软件：360管家，腾讯管家等，把app加入白名单，则清理时不会把app杀掉

## 华为的Android的离线推送

华为的Android端的离线推送叫做：HMS推送服务

根据官网教程去配置完后，即可。

在满足条件的华为设备上就可以使用华为推送接收离线推送通知了; 这里的满足条件是指：华为设备必须安装2.4以上的华为移动服务，以及开启当前 app 的自启动权限；

> 注意：华为EMUI 4.0需要把app自动启动权限打开才能收到推送。

详见：[GCM、华为推送 [环信开发文档]](http://docs.easemob.com/start/200androidcleintintegration/115payloadmsg)

## 小米的Android的离线推送

通过`MIUI`系统的支持，实现Android端的离线消息推送

详见：[小米开放平台 - 消息推送](https://dev.mi.com/console/appservice/push.html)
