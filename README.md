百度贴吧批量签到脚本
=====================

##说明

这是一个可以模拟客户端对百度贴吧进行批量签到的Python脚本。

修改自[idevcod的博文](http://blog.csdn.net/idevcod/article/details/11479897)(对应[Github仓库](https://github.com/ifreefly/baidu_bot))。对代码进行了完全重构，并改为可以模拟客户端进行签到。

模拟客户端部分参考了Userscript上的<del>[Tieba Client脚本](http://userscripts.org/scripts/review/177032)</del>(链接已失效）。
* 在Windows 8.1 与 Debian 上测试通过
* 在脚本所在目录生成一个简单的日志 tieba_log.log

##使用说明

* 适用于Python 2.7环境
* 通过浏览器抓包获取Cookie和BDUSS，获取BDUSS需要切换到 http://tieba.baidu.com/mo/ 注销并重新登陆
* 把脚本中的Cookie和BDUSS换成自己的值，然后执行脚本


##已知问题

<del>由于字符编码问题，Windows上输出会出现乱码，不过不影响本身签到功能。</del> 已修复
<del>为解决Windows上的乱码问题进行的修改导致在Linux/Debian上运行出现错误，正在试图加入系统环境判断，暂时可以使用baidu-tieba-auto-sign_linux.py<del> 已修复
在Linux上，如果关注贴吧数目过多，会出现“thread.error: can't start new thread”错误，会导致超出一定数目的贴吧没有签到，并且不生成日志，正在解决

##声明

本工具只用于研究和学习用途，不附带任何担保，请酌情使用。
