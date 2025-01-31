阿秀学长自己收集了一些不错的资料可以送给大家，大家可以按照自己的情况自行取用~

#### 1、良心推荐一个C++项目-基于跳表实现的数据库

**话说在前面，我可能是推荐这个 C++ 项目的第一人。**

毕竟 C++技术岗可以说是人均 WebServer 服务器的项目了。

去年找工作的时候，我也做了一个 Webserver 服务器项目，在学完 《C++ Primer》、《TCP/IP网络编程》和《Linux高性能服务器编程》后，在 TinyHttp 的基础上做了一个自己的 Webserver服务器，后来又发现了这个新的项目，我还真没看过有人推荐过它。



**写在前面**

该项目需要你有一定的 Redis 基础，如果Redis水平不好的话，最好先去看一下《 Redis设计与实现》和《Redis这两本书》，当当和京东 均有售。

如果需要这两本书的 PDF 版本的话，可以看一下这个电子书仓库，里面经典的计算机专业数据很多：https://github.com/forthespada/CS-Books



**推荐原因**

1、主要是 WebServer 烂大街了，感觉是个 C++党的简历上必有 WebServer 服务器，太千篇一律了。

2、该项目是与 Redis 中的跳表联系在一起，如果在面试中面试官谈起你的项目，很容易就会把话题扯到跳表上，进而跟 Redis 搭上线，而 Redis 数据库可以说是 后端开发必问的一个知识点了。

需要注意的是，千万不要自己对 Redis 一窍不通，还在简历上写了这个项目，因为很有可能面试官会借由这个项目问起你的 Redis 水平。



**项目介绍**

**基于跳表的数据库项目**

它是一个使用 C++ 编程实现的基于跳表的轻量级键值型数据库。提供的功能接口主要有插入元素、删除元素、查找元素、元素显示、元素清空、文件加载以及数据库大小显示。

看到这里很多人都会觉得low，觉得不过就是增删改查而已，是的，确实主要的功能就是增删改查。

但对于一些本科生，如果能将 C++ 、Redis、增删改查结合在一起也是很不容易的了，你又何尝不是每天CRUD呢..

![](https://cdn.jsdelivr.net/gh/forthespada/mediaImage1@1.6.3.9/202103/微信截图_20210311214549.png)

**性能测试**

插入元素测试

跳表高度为18的情况下，选择随机插入元素。当插入元素数量为 100,000 时，用时 0.316763 秒；当插入元素数量为 500,000 时，用时 1.86778 秒；当插入元素数量为 1000,000 时，用时 4.10648 秒；

查找元素测试

数据库全部元素为 100,000的 情况下，查找 10 个元素，耗时 0.47148 秒；

数据库全部元素为 500,000的 情况下，查找 20 个元素，耗时 2.56373 秒；

数据库全部元素为 1000,000的 情况下，查找 100 个元素，耗时 5.43207 秒；

编译步骤

```
make            // complie demo main.cpp
./bin/main      // run 
```

测试方式

```
sh stress_test_start.sh 
```

github地址：https://github.com/youngyangyang04/Skiplist-CPP

**再次提醒**

需要注意的是上面推荐的项目 需要你有一定的 Redis 基础，如果Redis水平不好的话，可以先去看一下《 Redis设计与实现》和《Redis这两本书》，当当和JD均有售。

##### **下载方式**

需要该项目的的小伙伴可以去阿秀学长的个人公众号「拓跋阿秀」或者扫描下方二维码，回复「**跳表**」即可获取，我已经下载好啦。

<div align="center"><img src="https://cdn.jsdelivr.net/gh/forthespada/mediaImage2@1.3/202103/公众号：拓跋阿秀.png" style="zoom:50%;" /></div>



#### 2、推荐其余的C++项目

我这两天又花时间整理了一下，推荐几个个人觉得还不错的 C++项目吧，由易到难。

##### 1、手把手教你从零开始实现一个 JSON

Json 是一个用于数据交换的文本格式 ，可用于任何编程语言。一个动态网页想从服务器获得数据时，服务器从数据库查找数据，然后把数据转换成 `JSON `文本格式：

`Json`格式如下：

>```json
>{
>"title": "Design Patterns",
>"subtitle": "Elements of Reusable Object-Oriented Software",
>"author": [
>   "Erich Gamma",
>   "Richard Helm",
>   "Ralph Johnson",
>   "John Vlissides"
>],
>"year": 2009,
>"weight": 1.8,
>"hardcover": true,
>"publisher": {
>   "Company": "Pearson Education",
>   "Country": "India"
>},
>"website": null
>}
>```

这个项目还可以，也是从 0 开始一步一步教你做的。作者是腾讯 T4   大佬， 曾参与《天涯明月刀》、《斗战神》、《爱丽丝：疯狂回归》等游戏项目 ，也是《C++ Primer 中文版（第五版）》的审校人之一，反正又是一个大佬，手动狗头。

>github链接：https://github.com/miloyip/json-tutorial

##### 2、实现属于你自己的 STL

一个合格的 `C++` 程序员是必须要会`STL`里的，其中的容器、算法在刷各种`OJ`的时候简直是一大利器。我知道有很多同学都有想过写一个属于自己的 `STL`，我也想过，但没行动过 hhh

MyTinySTL这个项目把我想的做了，它是基于 `C++11` 的` tinySTL`，其中实现了 大部分 `STL` 中的容器与函数 ，所以你也是完全可以照着它来实现自己的 `STL` 的。

>`github`链接：https://github.com/Alinshans/MyTinySTL

##### 3、烂大街的HTTP服务器

这个项目似乎成了Linux C/C++技术栈人手一个的项目了？

虽然这个项目烂大街了，看着也挺简单的，不过能玩的花样还是不少的。比如加入代理功能、添加支持 `CGI` 功能或者加入日志记录等。它越简单，你可以做的改进就越多，在面试的时候，你就可以跟面试官聊你的改进和你添加的功能，面试官是很愿意看到你的自己在做一个项目时的思考和改进的。偷偷跟你说，这种改进很加面试分的。

这里我推荐牛客大佬健康成长天线宝宝啊的 HTTP服务器，这位大佬现在在阿里云做平台开发。他在牛客上写的 `C++` 求职/基础架构路线文章非常不错，想要走 `C++` 路线的同学推荐你们去牛客看看他的帖子。

> 健康成长天线宝宝啊个人主页：https://www.nowcoder.com/profile/2765647?noredirect=true
>
> 健康成长天线宝宝啊服务器项目`github`链接：https://github.com/linyacool/WebServer

##### 4、实现一个多线程网络服务器 

这个是我在`github`上发现的，这里直接搬运一下该 `Demo` 的说明吧。

本项目为 `C++11` 编写的基于epoll 的多线程网络服务器框架，应用层实现了简单的`HTTP`服务器 ` HttpServer` 和一个回显服务器`EchoServer`，其中HTTP服务器实现了` HTTP`的解析和`Get`方法请求，目前支持静态资源访问，支持`HTTP`长连接；该框架不限于这两类服务器，用户可根据需要编写应用层服务。 

通过该项目你可以了解到部分 `C++11` 的语法和编码规范、学习巩固网络编程、网络 `IO` 模型、多线程、`git` 使用、`Linux`命令、性能分析、`TCP/IP、HTTP`协议等知识

>`github`链接：https://github.com/chenshuaihao/NetServer

##### 5、从0开始手把手教你做的服务器框架

说实话，这个算是比较难的`C++`项目了，是我在`B`站发现的，我看了底下的评论，相当不错。是一个C++ 高性能分布式服务器框架 的项目，我确认过了，是新手不要尝试的那种难度。

该项目主要有 13 大模块组成，分别是日志模块、配置模块、线程模块、协程模块、协程调度模块、`IO` 协程调度模块、`Hook` 模块、`Socket` 模块、`ByteArray` 序列化模块、`TcpServer `模块、`Stream` 模块、`HTTP` 模块、`Servlet` 模块。

>B站视频教程：https://www.bilibili.com/video/av53602631?from=search&seid=9029288577396826503
>
>服务器框架`github`链接：https://github.com/sylar-yin/sylar

##### 6、做个操作系统内核

《深入理解计算机系统》这本书大家应该都听说过吧，这本书被誉为“跟金子一样珍贵的计算机基础书籍”，如果你还没看过，赶快去买一本补补功课。

其中这本书中的一些`lab` 很是不错，你完全可以实现其中的一个小 `lab` 来作为自己的 C++』  项目的。而且这本书也是美国麻省理工学院的推荐的计算机书籍之一，课后的一些`lab` 也会布置给上课的学生。

想一下，面试官问你的项目背景是什么的时候，你直接告诉他“这是美国麻省理工学院的计算机专业学生的结课大作业”，**没有分量吗？不能装逼吗？**

建议先看一下 `B` 站 MIT 6.828  视频，再去实践。

>《深入理解计算机系统》课后`lab`作业`github`链接链接： https://github.com/woai3c/MIT6.828 



##### 下载方式

各位可以去github上直接克隆，如果觉得麻烦阿秀已经把上述六个项目下载打包好了。

需要该压缩包的的小伙伴可以去阿秀学长的个人公众号「**拓跋阿秀**」或者扫描下方二维码，回复「**项目**」即可获取。

<div align="center"><img src="https://cdn.jsdelivr.net/gh/forthespada/mediaImage2@1.3/202103/公众号：拓跋阿秀.png" style="zoom:50%;" /></div>























