### `DataGrid` 快捷键

之前一直使用 `navicat` , 后面用了 `datagrid` 之后, 可以说是爱不释手, 真的方便太多



#### **得到数据库创建 `SQL`**

选中对应表  - `ctrl + b`

![create-table-ddl-sql.png](http://193.112.98.8/atomImg/datagrid/create-table-ddl-sql.png)

#### 重命名表 `rename table`

选中对应表 - `shift + F6`

![rename-table.png](http://193.112.98.8/atomImg/datagrid/rename-table.png)



#### 更新表结构 `modify table`

选中对应表  - `ctrl + F6`

![](http://images.atomblogs.com/20190903205831.png)



#### 快速打开 `console` 可以输入命令操作指令

![open-console.png](http://193.112.98.8/atomImg/datagrid/open-console.png)

**运行命令**

![run-command.png](http://193.112.98.8/atomImg/datagrid/run-command.png)



#### 更快捷的方式 完美拥抱快捷键

> 有的时候, 会操作很多的表结构, 每次操作的时候都要来右键打开`console`, 说实话真的很烦
>
> 
>
> 由于 `GridFlow` 和 `IDEA` 出自同一公司, 所以他们的操作很多时候是一样的, 所以使用IDEA 基本可以非常流程的使用 `GridFlow`



##### 快速的查看某个表的数据

`ctrl + n`对比`idea` 查找类

![fast-select.png](http://193.112.98.8/atomImg/datagrid/fast-select.png)



##### 快速对表进行查找

> 以前每次使用`navicat` 的时候, 快速查找真的是一件很麻烦的事情

![fast-select-eg.png](http://193.112.98.8/atomImg/datagrid/fast-select-eg.png)

比如我们要检索文章标题中带有 `linux` 字样的文章, 在上方输入框中 输入 `title like '%linux%'`  按回车即可

![fast-select.png](http://193.112.98.8/atomImg/datagrid/fast-select.png)

#### 删除一条记录(与`Idea`中删除一行代码类似)

>  选中要删除行数据 `ctrl + y` , 这时这时标识你即将要删除的数据, 此时按下 `ctrl + enter`  确认删除



#### 添加一条相同的记录

> 有的时候我们在测试的时候可能需要比较多测试数据, 这时候就可以使用 `ctrl + d` 后使用 `ctrl + enter` 就可快速添加测试数据



#### 执行`sql`语句

> 以前的`navicat` 在执行语句的时候, 可能就是 选中当前行, 右键执行选中, 或者选中要执行的`sql` `ctrl + shift + R` , 但是在`GridFlow` 中 这项操作变得更加智能

- 如果在输入`sql`的界面中只有一条`Sql`的话, 直接使用 `ctrl + enter` , 便会执行这条语句

- 如果在界面中存在多条`sql`, 输入完毕后, 输入 `ctrl + enter` 那么会弹出让你选择执行的`sql`段, 默认选中当前段, 再次按`enter` 即可

  ![run-sql.png](http://193.112.98.8/atomImg/datagrid/run-sql.png)

> 这样就避免的选中 `sql` 实属神器



###  快速对比两个数据库差异

> 这个是真神器了, 在上线时对比测试环境和生产环境数据库之间存在的差异

按住 `ctrl` 选中要对比的数据库, 按 `ctrl + d`即可对比,

可以查看两个数据库之间的差距, 并生成对应的 `sql`

![](https://raw.githubusercontent.com/xiaoxiunique/Web-Tip/master/20191119085055.png)

![](https://raw.githubusercontent.com/xiaoxiunique/Web-Tip/master/20191119085358.png)

点击`Migrate Left` , 生成转化为右侧表对应的`Sql`

![](https://raw.githubusercontent.com/xiaoxiunique/Web-Tip/master/20191119085648.png)

