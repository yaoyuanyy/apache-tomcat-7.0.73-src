 ## tomcat-7.0.73源码解析
 
分析tomcat源码能更好的了解servlet原理和servlet容器；可以更直观的感受到.jsp是如何生成对应的.java和.class的；可以知道解析xml的一种方式：使用SAX；给我们展示最基本的服务框架的样子；给我们一种框架设计方式的展示；给我们线程池的用法等等。所以说，分析tomcat，能给我们很多的收益，而且是实实在在的。

网上有许多关于运行tomcat源码的文章，我下面也给出了链接。如果你想用现成的，能直接在ide上运行的tomcat源码项目，听我简要的说一下步骤：
- 在你本地要放置项目的文件路径中打开git客户端，粘贴命令：git clone https://github.com/yaoyuanyy/apache-tomcat-7.0.73-src.git,
- 通过ide导入刚克隆下来的项目
- 设置一下运行时的配置：我用的intellij，见下图：
![](https://github.com/yaoyuanyy/MarkdownPhotos/blob/master/tomcat/tomcat%E6%BA%90%E7%A0%81%E8%BF%90%E8%A1%8C%E5%89%8D%E9%85%8D%E7%BD%AE1.png?raw=true)
![](https://github.com/yaoyuanyy/MarkdownPhotos/blob/master/tomcat/tomcat%E6%BA%90%E7%A0%81%E8%BF%90%E8%A1%8C%E5%89%8D%E7%9A%84%E9%85%8D%E7%BD%AE2.png?raw=true)

配置后就可以在Bootstrap.java中点击右键->run/debug了，开始你的分析旅程吧
 
如果你想自己用intellij 搭建一个tomcat源码项目,详细步骤可参考：
* http://www.jianshu.com/p/9e3f99f2d5bb
* http://iamtiger.net/blog/2013/10/14/run-tomcat-in-idea-or-eclipse/


