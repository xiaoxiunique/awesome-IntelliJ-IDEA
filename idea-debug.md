Debug 用来追踪代码的运行流程，通常在程序运行过程中出现异常，启用 Debug 模式可以分析定位异常发生的位置，以及在运行过程中参数的变化。通常我们也可以启用 Debug 模式来跟踪代码的运行流程去学习三方框架的源码。



所以学习下如何在Intellij IDEA中使用好 Debug，主要包括如下内容：



## 断点

### 断点类型

IntelliJ IDEA中提供以下类型的断点：

- *行断点*：到达设置断点的代码行时挂起程序。可以在任何可执行代码行上设置此类断点。
- *方法断点*：在进入或退出指定方法或其实现之一时挂起程序，使您可以检查方法的进入/退出条件。
- *字段观察点*：读取或写入指定字段时挂起程序。这使您可以对与特定实例变量的交互做出反应。例如，如果在复杂过程的最后，您在其中一个字段上的值显然是错误的，则设置字段观察点可能有助于确定故障的来源。
- *异常断点*：`Throwable`抛出程序或其子类时挂起程序 。它们全局适用于异常条件，并且不需要特定的源代码引用。



### 添加断点

#### 设置行断点

单击要设置断点的可执行代码行中的装订线。或者，将插入号放在该行上，然后按⌘F8。

![image-20201211221911094](../.vuepress/public/image-20201211221911094.png)



如果该行包含lambda表达式，则可以选择是要设置常规的行断点，还是仅应在调用lambda时挂起程序。

![image-20201211221922048](../.vuepress/public/image-20201211221922048.png)

#### 设置方法断点

单击声明方法所在行的装订线。或者，将插入号放在该行上，然后按⌘F8。

![image-20201211221935900](../.vuepress/public/image-20201211221935900.png)

要在调用某个类的默认构造函数时挂起程序，请在声明该类的行上单击装订线，或在该行处插入插入符号，然后按 ⌘F8。

![image-20201211222054855](../.vuepress/public/image-20201211222054855.png)



#### 批量添加断点

要匹配多个类或方法，请 在“**调试”**工具窗口的左侧单击“ **查看断点”** ，然后单击“ **添加”** 并指定类和方法。

<img src="../.vuepress/public/image-20201211092816766.png" alt="image-20201211092816766" style="zoom:67%;" />

#### 设置字段 监听

![img](https://resources.jetbrains.com/help/img/idea/2020.3/debug_field_watchpoint.png)





### 移动/ 复制断点

![idea_move_copy_breakpoints](C:/Users/atom.hu/Desktop/idea_move_copy_breakpoints.gif)





### 删除断点

![idea_remove_breakpoints](../.vuepress/public/idea_remove_breakpoints.gif)



### 启动和禁用断点

有的时候 我们虽然设置了断点，但是我们临时 不想使用断点了

![idea_disable_breakpoints](../.vuepress/public/idea_disable_breakpoints.gif)



### 配置断点属性

在我们进行调试的时候，很多时候其实并不需要所有断点发生情况都触发，我们需要有条件的触发，这个时候我们就可以为这个断点本生设置条件，只有在条件范围内触发后 在触发断点。

![idea_condition_breakpoints](../.vuepress/public/idea_condition_breakpoints.gif)



### 无阻塞断点

<img src="../.vuepress/public/image-20201211222523554.png" alt="image-20201211222523554" style="zoom:50%;" />

- 断点 图示 

![image-20201211222907248](../.vuepress/public/image-20201211222907248.png)



## Debug Tool Windows

默认情况下，当您的程序遇到断点时，“**调试**工具”窗口将打开，而在会话终止时则不会隐藏。要更改此行为，请清除 “构建，执行，部署” |在断点**上**显示调试窗口在断点上”**复选框。**设置/首选项的 **调试器**页面。 

![image-20201211223041504](../.vuepress/public/image-20201211223041504.png)



### 会话

![image-20201211223101186](../.vuepress/public/image-20201211223101186.png)



如果为特定的运行/调试配置启用“服务”窗口，则在调试这些配置时，“调试”窗口的整个视图将显示在“服务”窗口中。

所选会话选项卡将显示所有信息，如内联变量值和执行点。如果要并行运行多个使用相同类的调试会话，则这一点很重要。



![image-20201211223127034](../.vuepress/public/image-20201211223127034.png)



### 标签

<img src="../.vuepress/public/image-20201211223834062.png" alt="image-20201211223834062" style="zoom:50%;" />



**调试**工具窗口为每个会话显示以下选项卡：

- Frames：使您可以在线程的调用堆栈中导航。

- Variables：列出当前上下文中可用的变量，并让您分析和修改程序状态。

- Watches：让您管理手表。默认情况下，监视显示在“**变量”**选项卡上，以更有效地利用屏幕空间。如果您有很多手表，请考虑在单独的标签中查看它们。

- Console：显示程序输出。

  对于本地会话，该选项卡的作用与您在未连接调试器的情况下运行该程序的作用相同。唯一的区别是调试器输出（例如，来自断点的日志消息）已添加到控制台。

  当您附加到进程时，程序输出不会重定向，并且调试器控制台中仅显示调试器输出。

- Threads：显示活动线程列表，并允许您在它们之间切换。在此选项卡中，您可以以文本格式导出线程信息。

- Memory：提供有关堆上当前可用对象的信息，并允许您监视和分析它们的生存期。

- Overhead：允许您监视特定调试器功能消耗的资源并优化调试器性能。



### 显示/隐藏标签

<img src="../.vuepress/public/debug_overview_show_tabs.png"/>



### 移动标签

<img src="../.vuepress/public/debug_move_tabs.png"/>



### 恢复默认布局

<img src="../.vuepress/public/debug_restore_layout.png"/>



## 断点 TopTips

- 无代码打印日志
- 通过断点判断程序执行时长
- Overhead
- Remote Debug
- 监听 JVM Heap

- Debug开篇

- 基本用法&快捷键

- 变量查看

- 计算表达式

-  智能步入

- 断点条件设置

- 多线程调试

- 回退断点

- 中断Debug