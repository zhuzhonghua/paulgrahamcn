---
layout: post
title : "世界上最危险的代码(The most dangerous code in the world)"
category : hackernews
tags : [hackernews]
---
{% include JB/setup %}

[在非浏览器软件里验证SSL证书](http://news.ycombinator.com/item?id=4695350)

摘要:
SSL (Secure Sockets Layer)是安全网络通信标准。在网络攻击中，安全的SSL连接取决于在建立连接时正确验证公钥证书。我们演示了SSL证书验证在高安全性的程序和类库中是完全可以打破的。包括基于SSL的Amazon EC2 Java库和所有云客户端等等脆弱的软件；负责传送电子商务网站的商户支付细节到支付网关的Amazon的SDK和PayPal；综合购物车如osCommerce, ZenCart, Ubercart, and PrestaShop; 移动网站使用的AdMob代码;移动银行和好几个Android程序和类库；Java Web服务中间件——包括Apache Axis,Axis 2,Codehaus XFire和Android的推送类库——还有所有使用这些中间件的程序.对于一个在中间攻击的人来说，任何从这些程序过来的SSL连接都是不安全的.这些安全漏洞的根源是SSL实现(如JSSE,OpenSSL,GnuTLS)的稀烂APIs和展现给开发者一堆有迷惑性的设定和选项的数据传输库(比如cURL).我们分析了这些软件中基于这些API的SSL证书验证的危险和陷阱，并且提出了我们的建议。
