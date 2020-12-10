## 设置工具窗口



### 移动工具窗口

默认情况下，工具窗口附加到主窗口的边缘。您可以分离它们以作为单独的窗口使用，如“工具”窗口视图模式中所述。



- 单击并拖动工具窗口栏上的工具窗口按钮。

- 或者，您可以单击工具窗口选项菜单，或者右键单击工具窗口标题栏，然后在“移动到”下选择附加工具窗口的位置。

  ![Tool window options menu: Move to](../.vuepress/public/tool-window-moveto.png)

### 调整工具窗口大小



- 单击并拖动工具窗口的边框。

要按步骤调整活动工具窗口的大小，请从主菜单中选择相应的操作，默认指定为以下快捷方式: 

>  Mac  | ⇧⌘←, ⇧⌘→, ⇧⌘↑, ⇧⌘↓.

![image-20201208233236955](../.vuepress/public/image-20201208233236955.png)

⇧⌘→ 输入两次

![image-20201208233306933](../.vuepress/public/image-20201208233306933.png)



要将工具窗口拉伸到最大宽度或高度，请按 ⇧⌘ ' 或从主菜单中选择 Window | Active Tool Window | Resize | Maximize Tool Window。

> 这个在查询错误日志的时候特别方便，这个时候就可以将 Debug Tool Windows 调整到最大，查看错误日志



![image-20201208233552854](../.vuepress/public/image-20201208233552854.png)

 `⇧⌘ '`

![image-20201208233621672](../.vuepress/public/image-20201208233621672.png)

上面就已经将工具栏放置最大了。



### 恢复工具箱的默认配置

可以设置，就肯定可以重置设置

在主菜单中，选择 Window | Restore Default Layout 或者按 ⇧⌘ F12。



### 保存现有工具窗口的配置

在主菜单中，选择 Window | Store Current Layout as Default。





### 针对宽屏显示器进行优化

Intellijidea 提供了几个选项来优化工具窗口在宽屏幕显示器上的位置。

- 在设置/首选项对话框 something 中，选择外观和行为 | 外观。

- 在工具窗口下，配置如下:

  宽屏工具窗口布局: 通过限制水平工具窗口的宽度，使垂直工具窗口的高度最大化。

  

  **关闭优化**

  ![The Widescreen tool window layout option is disabled](../.vuepress/public/WideScreenOFF.png)

  

  **开启优化**

  ![The Widescreen tool window layout option is enabled](../.vuepress/public/WideScreenON.png)

- 启用以两列显示垂直工具窗口，而不是将它们堆叠在一起。

  **开启前**

  ![Side-by-side layout is off](../.vuepress/public/side_by_side_left_off.png)

  

  **开启后**

  ![Side-by-side layout is on](../.vuepress/public/side_by_side_left.png)