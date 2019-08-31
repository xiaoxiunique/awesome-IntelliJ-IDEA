
### idea 插件

**Alibaba Cloud Toolkit**

个人经常会有这样的需求, 每次自己更新完测试环境之后, 就需要 `maven` 打包`clean install`, 然后`copy` `jar` 包, 利用`ftp`工具上传`jar`包到测试服务器, 然后`kill` 服务, 在启动服务 `java -jar` , 有时更新频繁 这就是一件非常麻烦的事

`Cloud Toolkit` 是本地 `IDE` 插件，帮助开发者更高效地开发、测试、诊断并部署应用。通过插件，您可以将本地应用一键部署到云端`（ECS、EDAS 和 Kubernetes 等`）和任意服务器；并且它还内置了 `Arthas` 程序诊断、`Dubbo工具`、`Terminal Shell` 终端和 `MySQL` 执行器等工具。

[官网链接](https://www.aliyun.com/product/cloudtoolkit)

简单的说, 安装了这个插件之后, `idea` 就具备了一些`jenkins`的自动部署的功能

**0x01** 安装

在 `idea` 工具中` Plugins` 直接搜索安装

**0x02** 使用


在安装完成之后, 在工具栏中就会出现阿里云的按钮, **点击按钮**

![](http://images.atomblogs.com/atom/20190831235312.png?img)


然后点击 `Deploy to Host`, 然后下方就会出现添加主机页面
![](http://images.atomblogs.com/atom/20190831235513.png?img)


点击 `Add Host`

![](http://images.atomblogs.com/atom/20190831235536.png?img)

以我自己的[博客](www.atomblogs.com)为例, 输入完配置之后, 点击 `Test Connection`, 出现 `Succeeded`, 点击 `add`, 代表添加成功

![](http://images.atomblogs.com/atom/20190831235554.png?img)

然后再点击 `Deploy to Host`

![](http://images.atomblogs.com/atom/20190831235602.png?img)

点击`Run`, `idea` 便会, 先使用`maven`打包, 后发送到服务器的指定位置

![](http://images.atomblogs.com/atom/20190831235612.png?img)

![](http://images.atomblogs.com/atom/20190831235621.png?img)

后续还可以 监听启动日志, 很简单, 就是 `Advanced` 里面, 大家看看就知道了, 
后续有时间再完善笔记吧

**阿里巴巴编码规范**
```
Alibaba Java Coding Guidelines 
```

**翻译插件**
```
Translation
```

**mybatis 插件**
```
Free Mybatis plugin
```

**Lombok 插件**
```
IntelliJ Lombok plugin
```

**Lombok pom.xml 文件配置**
```
<dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <version>1.16.18</version>
    <scope>provided</scope>
</dependency>
```
**GenAllSetter 特性**

在`Java`方法中, 根据 `new` 关键词, 为`Java Bean` 生成所有`Setter`方法。

按`GenAllSetter`键两次, 会为`Setter`方法生成默认值。


**GenDaoCode**

一键生成 `dao` `xml` `service`

**CodeGlance**

在右侧生成代码地图


**RestfulToolkit**

`RequestMapping搜索神器`

**Grep Console**

高亮`log`不同级别日志，看日志的时候一目了然。

**MyBatis Log Plugin**

把 Mybatis 输出的sql日志还原成完整的sql语句，看起来更直观。
