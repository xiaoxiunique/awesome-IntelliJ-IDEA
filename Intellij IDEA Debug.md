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

![img](file://F:/%E6%88%91%E7%9A%84%E5%9D%9A%E6%9E%9C%E4%BA%91/%E7%8E%A9%E8%BD%AC%20IDEA/.vuepress/public/debug_line_breakpoint.png?lastModify=1607649891)



如果该行包含lambda表达式，则可以选择是要设置常规的行断点，还是仅应在调用lambda时挂起程序。

![img](file://F:/%E6%88%91%E7%9A%84%E5%9D%9A%E6%9E%9C%E4%BA%91/%E7%8E%A9%E8%BD%AC%20IDEA/.vuepress/public/debug_breakpoints_lambda.png?lastModify=1607649960)

#### 设置方法断点

单击声明方法所在行的装订线。或者，将插入号放在该行上，然后按⌘F8。

![img](file://F:/%E6%88%91%E7%9A%84%E5%9D%9A%E6%9E%9C%E4%BA%91/%E7%8E%A9%E8%BD%AC%20IDEA/.vuepress/public/debug_method_breakpoint.png?lastModify=1607649988)

要在调用某个类的默认构造函数时挂起程序，请在声明该类的行上单击装订线，或在该行处插入插入符号，然后按 ⌘F8。

![img](file://F:/%E6%88%91%E7%9A%84%E5%9D%9A%E6%9E%9C%E4%BA%91/%E7%8E%A9%E8%BD%AC%20IDEA/.vuepress/public/debug_constructor_breakpoint.png?lastModify=1607650006)





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

![idea_disable_breakpoints](C:/Users/atom.hu/Desktop/idea_disable_breakpoints.gif)



### 配置断点属性

在我们进行调试的时候，很多时候其实并不需要所有断点发生情况都触发，我们需要有条件的触发，这个时候我们就可以为这个断点本生设置条件，只有在条件范围内触发后 在触发断点。

![idea_condition_breakpoints](C:/Users/atom.hu/Desktop/idea_condition_breakpoints.gif)



### 无阻塞断点



- 断点 图示 



## Debug Tool Windows

Debug 工具窗介绍





## 断点 TopTips

- 无代码打印日志
- 通过断点判断程序执行时长
- Overhead
- Remote Debug
- 监听 JVM Heap
- 





- Debug开篇

- 基本用法&快捷键

- 变量查看

- 计算表达式

-  智能步入

- 断点条件设置

- 多线程调试

- 回退断点

- 中断Debug