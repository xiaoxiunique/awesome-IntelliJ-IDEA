### idea 快捷键
#### 通用类快捷键

**方法参数提示**
```
ctrl + p
```
![image](10125A47B2344D7B99B39C1A7059AB4D)

**折叠代码**
```
ctrl + -
```
![image](8520B722A8F840D7904570798C7BDC35)
**全局查找文本**

```
ctrl + shift + F
```


**快速查找和打开最近使用过的文件码**
```
ctrl + E
```
![](![image](10B8BE278DA54E4EAEB81A619E9F673D))

**自动代码片**
```
ctrl + j
```
![image](F956E0046E78419F9D905BED371D3EEF)

**实现接口方法**
```
ctrl + i
```

![image](822FA91B16764DB199176C81EDD16D9A)


**查看当前类的子类**
```
ctrl + h
```


**将当前行和下一行进行合并**
```
ctrl + shfit + j
```


**将光标跳到当前行的上一行**

有时候在写完一行代码的时候需要添加注释, 或者为类属性添加注释的时候需要跳到当前行的上一行, 这个快捷键就非常方便

```
ctrl + alt + enter
```


**idea git 提交**
```
ctrl + k
```
![image](43C827E6D3754B1497717AF44A2FF8E8)

**删除当前行**
```
ctrl + y
```
**重写 或者 实现接口或父类方法**
```
ctrl + o
```

**显示类之间的关系**
```
ctrl + alt + u
```
![image](CEC45F36893749EB9F370684D39A08D8)
**删除类中没有用到的package**
```
ctrl + alt + o
```

**进入设置界面**
```
ctrl + alt + s
```
![image](BB6286E2E862478A88016F00730E8F61)

**在当前光标在的这样一行的下一行添加一行**
```
ctrl + shfit +enter
```

**弹出， 当前类中的方法集合**
```
ctrl + F12
```
![image](468D074207AE4ADB901D2866AA56BD2A)
**添加书签**
```
ctrl + f11
```

**比较强大的几个快捷键之一  Ctrl + ~(感叹号旁边的按键)**
```
ctrl + ~
```
**共有五种可供选择的操作**

**Switch Code Formatter (切换代码格式化程序)**
可以在eclipse和idea的代码格式化之间快速转换

**Color Scheme (配色方案)**
可以设置一些常用的配色, 字体样式, 可以一键切换

**Code Style Scheme **


**Keymap (快捷键列表)**
**View Mode (显示模式)**
**Look and Feel (设置软件主题)**

**搜索文件**
```
ctrl + shift + n
```
![image](C41EC33E9F474CF3AD4A4167A0D4546B)
**搜索类合**
```
ctrl + n
```
![image](A6B1928C4DC34EE99A1E80468CB3050E)
**抽取局部变量**
```
ctrl + alt + v
```
**进入到实现子类中**
```
ctrl + alt + b
```
![image](D7757E9131554456B20BD89143D06243)

**格式化代码**
```
ctrl + alt + L
```

**idea 多光标选择**
```
按下滚轮上下拖动鼠标即可，
```

**运行当前类**
```
ctrl + shift + F10
```

**从多项目中启动一个 debug 模式**
```
alt + shfit + F9
```


**从多项目中启动一个 正常模式**
```
alt + shfit + F10
```



**idea 调出版本控制操作**
```
alt + ~
```

![image](5BE55A1ED07E4E5F8C3A1E8FDE670EE7)

**idea ssh 工具**

平常在开发的时候, 避免不了需要远程服务器操作, 平常我们可能会使用 `xshell` 等连接工具, 但是其实 `idea`也内置了这样的功能

![image](6EB6C9A7C43D4A8EAC81251E3426781B)

![image](A8F6103E5DC84E5A95A2EE41AAD7D764)

上图中展示的是 `IDEA` 中两个非常棒的内置功能，可以在 `Tools -> Start SSH session` 中开启远程服务器的终端，在` IDEA` 下方可以执行远程指令；也可以在 `Tools -> Deployment ->Browse Remote Host` 中展开如图右侧的结构，可视化地浏览服务器上的文件列表，检查应用是否部署成功。


### idea 插件

**Alibaba Cloud Toolkit**

个人经常会有这样的需求, 每次自己更新完测试环境之后, 就需要 `maven` 打包`clean install`, 然后`copy` `jar` 包, 利用`ftp`工具上传`jar`包到测试服务器, 然后`kill` 服务, 在启动服务 `java -jar` , 有时更新频繁 这就是一件非常麻烦的事

`Cloud Toolkit` 是本地 `IDE` 插件，帮助开发者更高效地开发、测试、诊断并部署应用。通过插件，您可以将本地应用一键部署到云端`（ECS、EDAS 和 Kubernetes 等`）和任意服务器；并且它还内置了 `Arthas` 程序诊断、`Dubbo工具`、`Terminal Shell` 终端和 `MySQL` 执行器等工具。

[官网链接](https://www.aliyun.com/product/cloudtoolkit)

简单的说, 安装了这个插件之后, `idea` 就具备了一些`jenkins`的自动部署的功能

**0x01** 安装

在 `idea` 工具中` Plugins` 直接搜索安装

**0x02** 使用

![image](7C687AC7304E43618EEA477ACD47A352)

在安装完成之后, 在工具栏中就会出现阿里云的按钮, **点击按钮**

![image](E83C5BF5EE4D44728AED18FBE379D53A)

然后点击 `Deploy to Host`, 然后下方就会出现添加主机页面

![image](9FE7017D4B584FAC84B8EE7B43FA22C3)

点击 `Add Host`

![image](ABAA7BE958074CE2AD7C39C957B59CB1)

以我自己的[博客](www.atomblogs.com)为例, 输入完配置之后, 点击 `Test Connection`, 出现 `Succeeded`, 点击 `add`, 代表添加成功

![image](92FB3B36F45449A18C26191E861AC6E9)

然后再点击 `Deploy to Host`

![image](5D09875C82A1481FA23B8C642C9C64B9)

点击`Run`, `idea` 便会, 先使用`maven`打包, 后发送到服务器的指定位置

![image](09099B3ECAEB48D19EFBB33D451E60A5)

![image](0D9AFE2CA2264EB991E762A259F48200)

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

在Java方法中, 根据 new 关键词, 为Java Bean 生成所有Setter方法。

按GenAllSetter键两次, 会为Setter方法生成默认值。


**GenDaoCode**

一键生成 `dao` `xml` `service`

**CodeGlance**

在右侧生成代码地图


**RestfulToolkit**

`RequestMapping搜索神器`

**Grep Console**

高亮log不同级别日志，看日志的时候一目了然。

**MyBatis Log Plugin**

把 Mybatis 输出的sql日志还原成完整的sql语句，看起来更直观。
