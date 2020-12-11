### IDEA 常用设置

##### `0x01` **IDEA以新窗口的形式打开多个项目**

> File - Settings - Appearance & Behavior - System Settings

![setting-multiple.png](http://193.112.98.8/atomImg/setting/setting-multiple.png)

##### `0x02` 修改IDEA 默认编码 -> UTF-8

> File - Settings - Editor - File Encodings

![setting-encoding.png](http://193.112.98.8/atomImg/setting/setting-encoding.png)

##### `0x03` 设置统一编译器和编译版本

> File - Setting - Build - Compiler - Java Compiler

![setting-compiler.png](http://193.112.98.8/atomImg/setting/setting-compiler.png)

##### `0x04` 设置类注释

> File - Editor- File and Code Templates

```java
/**
* @Package ${PACKAGE_NAME}
* @author atom.hu
* @date ${DATE} ${TIME}
* @version V1.0
*/
```

![setting-class-comment.png](http://193.112.98.8/atomImg/setting/setting-class-comment.png)



`$$end$$` 可以设置光标结束的位置



##### `0x05` 自动导包

> File - Editor- General - Auto Import

![setting-auto-import.png](http://193.112.98.8/atomImg/setting/setting-auto-import.png)

##### `0x06` 内存使用量展示

> 由于日常开发时都是在公司的办公电脑上进行的，所以内存总是不够用，但是又不清楚IDEA具体实时的占用了多少内存。这个时候对于一些内存并不是太够的开发人员来说能看到实时的内存使用量还是比较好的
>
> File - Settings - Appearance & Behavior

![setting-use-memory.png](http://193.112.98.8/atomImg/setting/setting-use-memory.png)

![](http://images.atomblogs.com/atom/20190831212401.png?img)

##### `0x07` 开启悬浮提示

> 有时候在看代码的时候，不清楚一个类具体是干什么的，就会点进去看这个类的注释，但是强大的IDEA是支持不用点进去就可以看到注释的以及类的相关信息的。
>
> File - Settings - Editor - General

![setting-enable-hover-tip.png](http://193.112.98.8/atomImg/setting/setting-enable-hover-tip.png)

##### `0x08` Ctrl+鼠标滚轴修改字体大小

> IDEA也支持向浏览器那样按住Ctrl+鼠标滚轴来改变编辑区的字体的大小
>
> File-->Settings-->Editor-->General。

![setting-mouse-change-font.png](http://193.112.98.8/atomImg/setting/setting-mouse-change-font.png)

##### `0x09` 显示多行Tab

> 当我们打开的标签页多了的时候，默认的会隐藏在右侧，当我们需要的时候在右侧找到后再打开。IDEA是支持多行显示的，这样在大屏幕的显示器上也不用总去点击右侧的去找刚才打开过的文件了
>
> File - Settings - Editor - General - Editor Tabs

![setting-multiple-tab.png](http://193.112.98.8/atomImg/setting/setting-multiple-tab.png)

##### `0x0A` 设置字体, 行距 让代码看着更舒服

> File - Settings - Editor - Font

![setting-change-font-padding.png](http://193.112.98.8/atomImg/setting/setting-change-font-padding.png)

##### `0x0B` IDEA GIT 配置

>  File - Settings - Version Control - Git

![setting-git-config.png](http://193.112.98.8/atomImg/setting/setting-git-config.png)

##### `0X0C` IDEA MAVEN 配置

> File - Settings - Build - Build Tools - Maven

#####  ![setting-maven-setting.png](http://193.112.98.8/atomImg/setting/setting-maven-setting.png)

maven 阿里镜像配置

```xml
<mirror>
    <id>nexus</id>
    <mirrorOf>*</mirrorOf> 
    <url>http://maven.aliyun.com/nexus/content/groups/public/</url>
</mirror>
```

