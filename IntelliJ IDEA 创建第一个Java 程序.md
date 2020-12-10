在本教程中，您将学习如何创建、运行和打包一个打印 Hello，World 的简单 Java 应用程序！到系统输出。在此过程中，您将熟悉 IntelliJ IDEA 特性，以提高作为开发人员的工作效率: 编码辅助和补充工具。



## 准备一个项目

### 创建一个新的 Java 项目

在 IntelliJ IDEA 中，一个项目可以帮助您将源代码、测试、使用的库、构建说明和个人设置组织到一个单元中。

1. 启动 IntelliJ IDEA。

   如果打开欢迎屏幕，请单击“新建项目”。

   否则，从主菜单中选择 File | New | Project。

   

2. 在 New Project 向导中，从左侧的列表中选择 Java。

   

3. 要在 intellijidea 中开发 Java 应用程序，您需要 javasdk (JDK)。

   如果所需的 JDK 已经在 IntelliJ IDEA 中定义，那么从 Project SDK 列表中选择它。

   如果 JDK 安装在您的计算机上，但是没有在 IDE 中定义，那么选择 Add JDK 并指定 JDK home 目录的路径(例如,/library/java/javavialmachines/JDK-13.0.1)。Jdk).

   ![image-20201211000350398](../.vuepress/public/image-20201211000350398.png)

   如果您的计算机上没有必要的 JDK，选择 Download JDK。在下一个对话框中，指定 JDK 供应商(例如 OpenJDK)、版本，如果需要则更改安装路径，然后单击 Download。

   ![Downloading a JDK when creating a project](../.vuepress/public/download-jdk.png)

   

4. 在本教程中，我们不打算使用任何其他库或框架，因此请单击“下一步”。

   

5. 不要从模板创建项目。在本教程中，我们将从头开始执行所有操作，因此请单击“下一步”。

   

6. 为项目命名，例如：HelloWorld。

   

7. 如有必要，请更改默认项目位置并单击“完成”。

   ![48ce293f-c617-42b9-8313-8f6db998604b](../.vuepress/public/48ce293f-c617-42b9-8313-8f6db998604b-1607334071520.gif)



### 创建 package 和 class



包用于将属于同一类别或提供类似功能的类组合在一起，用于构造和组织具有数百个类的大型应用程序。



1. 在 Project 工具窗口中，选择 src 文件夹，按 Alt + Insert，然后选择 Java Class

   

2. 在 Name 字段中，键入 com.example.HelloWorld. HelloWorld 并单击 OK. IntelliJ IDEA 创建 com.example.HelloWorld 包和 HelloWorld 类。

   

   ![48ce293f-c617-42b9-8313-8f6db998604b](../.vuepress/public/48ce293f-c617-42b9-8313-8f6db998604b.gif)

   与该文件一起，IntelliJ IDEA 自动为您的类生成了一些内容。在这种情况下，IDE 插入了包语句和类声明。这是通过文件模板来完成的。根据您创建的文件的类型，IDE 插入初始代码和预期在该类型的所有文件中存在的格式。有关如何使用和配置模板的详细信息，请参阅文件模板。



### 开始编码

通过动态模板增加 main 方法

![5eedd822-581b-4af7-8bee-67c70cf4ee50](../.vuepress/public/5eedd822-581b-4af7-8bee-67c70cf4ee50.gif)



### 输出 print 方法

![26dc1490-7527-4c01-a19f-959de550da2e](../.vuepress/public/26dc1490-7527-4c01-a19f-959de550da2e.gif)



### 运行方法

![82c13843-d559-4200-8ced-bda71d1c0e7a](../.vuepress/public/82c13843-d559-4200-8ced-bda71d1c0e7a.gif)



### 将工程打包为 Jar 包

![98133f10-7b16-444e-9a9e-4144e067a4d5](../.vuepress/public/98133f10-7b16-444e-9a9e-4144e067a4d5.gif)



如果你能看到 `out/artifacts` 文件夹，那么你将能看到 Jar 包

![jt-jar-built](../.vuepress/public/jt-jar-built.png)



### 运行打包的应用程序



### 执行 Jar

