# douyudanmu
斗鱼直播间弹幕爬取python

![image](https://github.com/shuishen49/douyudanmu/blob/master/01.PNG?raw=true)

 我最近在学习python的直播间弹幕爬取，但是由于斗鱼官方把第三方api的接口改变了，必须要注册为开发者才能使用官方提供的方法进行弹幕爬取。所以我通过搜索教程了解到可以使用浏览器自带的爬取功能对弹幕进行爬取。

原理如下：

利用websocket建立wss 连接

wss://danmuproxy.douyu.com:8506/'

8501-8507都可以使用。

发送登录信息

发生入组信息

发送心跳数据，（和b站不一样更高级了，有心跳数据了）。

利用wss必须对发送包进行加密，对接收的数据进行解包，

这些操作官方api 有提供，所以我就不再进行解释了。

就能返回弹幕数据。

将roomid = "666743" 改成你需要的id。
