百度贴吧批量签到脚本
=====================

##说明

这是一个可以模拟客户端对百度贴吧进行批量签到的Python脚本。

修改自[idevcod的博文](http://blog.csdn.net/idevcod/article/details/11479897)(对应[Github仓库](https://github.com/ifreefly/baidu_bot))。对代码进行了完全重构，并改为可以模拟客户端进行签到。

模拟客户端部分参考了Userscript上的<del>[Tieba Client脚本](http://userscripts.org/scripts/review/177032)</del>(链接已失效）。


##使用说明

* 适用于Python 2.7环境
* 通过浏览器抓包获取Cookie和BDUSS，获取BDUSS需要切换到 http://tieba.baidu.com/mo/ 注销并重新登陆
* 把脚本中的Cookie和BDUSS换成自己的值，然后执行脚本


##已知问题

由于字符编码问题，Windows上输出会出现乱码，不过不影响本身签到功能。

##声明

本工具只用于研究和学习用途，不附带任何担保，请酌情使用。
