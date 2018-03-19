前一段时间我们公司业务相关刚好也用到了这个技术，我们几个技术苦逼地熬夜也是在网上疯狂地找这方面的相关资料，发现这块技术更新非常快，很多都是以前能用现在不能用的，还有很多家伙技术牛的弄出来了过去问也是藏着掖着，技术共享才有进步啊，不过还好最后还是让我们几个给弄出来了，现在就分享给大家。
跳转原理分析：
从手机浏览器等非微信环境，跳转到微信，都是利用weixin://dl/business/?ticket=ta42491d55a5fae0e143599655f2efe6e 这种形式的微信scheme。微信为了让京东，美团大的合作商家能直接跳转到微信，都给了他们生成跳转微信接口。跳转的原理，就是利用微信提供给这些商家的接口，把我们的链接转换成对应的ticket链接。

在哪儿可以找到微信跳转的接口呢？我们分析跳转链接后，发现了接口的出处。
接口地址：[http://www.tdcq.me](http://www.tdcq.me/)
（后来才得知这个地址是不定期对外开放的，能不能访问看运气） 
到网站上可以申请到微信跳转接口，然后直接调用他们提供的接口，就可以把我们的链接转换成对应的微信跳转链接了。

微信跳转这块有什么问题，可以加我QQ：53285820，一起沟通交流微信跳转技术。



微信跳转技术，扫描二维码可立即在微信打开宣传落地页！详情请点击www.tdcq.com了解！