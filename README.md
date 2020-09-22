##什么是PowerMTA？

PowerMTA是功能强大的MTA软件（SMTP），用于通过Internet发送电子邮件，可以使每天单台服务器可投递百万级邮件。

##什么是Mumara？

几年前网上流行的版本都是PMTA + OEMPRO ，但这已经过时了，现在我们可以使用Mumara替代OEMPRO，Mumara是一种邮件营销一体化的前端,可以通过网页端发送给你的客户你想要发送的内容.

准备工具：
1、PowerMta5.0一键安装包
2、域名
3、准备一台VPS(当然独立服务器更好啦)，系统Centos7.x 64位版本。（服务器一定要是25端口打开了的，否则会发不出去邮件）


开始安装：
1、![image.png](https://upload-images.jianshu.io/upload_images/1677613-3ecee73f45573131.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
      这里有五个选项，123都是网页前端，不需要的话可以选择5，这里我们使用前端Mumara.
2、输入许可证之后会让你输入你的域名
3、接着安装脚本的指示输入提示信息然后等待自动安装就可以了。

![QQ截图20200922201212.png](https://upload-images.jianshu.io/upload_images/1677613-3577f8f5853fe1ae.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
这样就算是安装完成了，接下就是把dkim，spf这些配置到域名dns就可以了。

![QQ123.png](https://upload-images.jianshu.io/upload_images/1677613-112a402cfc37b7da.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这里在域名dns把我们的服务器IP配置上就算完成了。接下来就可以测试发邮件了。

测试发件：

1、我们先使用smtp软件测试发送。
  ![123.png](https://upload-images.jianshu.io/upload_images/1677613-bb8196c0b5482806.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

显示发送成功，来自我们搭建的邮箱和域名。

![image.png](https://upload-images.jianshu.io/upload_images/1677613-ee64d167a8177321.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

也可以通过网页看到我们发送的数据

2、还有一种就是通过网页版发送，也就是Muamara发送。
  
![image.png](https://upload-images.jianshu.io/upload_images/1677613-a8366a9e1f6f937c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这是后台操作页面。

![QQ图片20200923000639.png](https://upload-images.jianshu.io/upload_images/1677613-09a36148a9794dd7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![image.png](https://upload-images.jianshu.io/upload_images/1677613-7b08e890bc68b053.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

网页版测试发送了三封也发送成功并进了收件箱。

有兴趣的可以联系我的VX:sunoath。



