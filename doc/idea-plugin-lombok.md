## Intellij IDEA 插件 Lombok

生命很宝贵, 没有必要浪费在这个重复的工作上, 尤其是如果我们使用传统的 `get` `set` 方法, 在实体类进行变更的时候, 或多添加了列, 或减少了列, 又要重新生成对应的 `get set` 这难道不就是浪费时间浪费生命吗?



```xml
<dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <version>1.16.18</version>
    <scope>provided</scope>
</dependency>
```



还不熟悉使用的可以看这篇文章

[Java 开发之 Lombok 必知必会](https://juejin.im/post/5cf3edf7e51d454f71439c79)