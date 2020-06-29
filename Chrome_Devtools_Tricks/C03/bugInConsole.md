::: quote
用 `console.log()` 来打印一个修改过的对象，修改前后打印的结果，竟然是一样的？
:::

### 1.例子

![](https://wingman-1300536089.cos.ap-shanghai.myqcloud.com/chrome/C03/async_console.gif)

最后一次执行的代码，我们再修改的前后打印同一个对象，但打印的时候，为什么都是修改之后的值呢？

如果你细心一点你就会发现右边有一个小小的 `i` 符号，把鼠标放上去就可以看到原因：

![](https://wingman-1300536089.cos.ap-shanghai.myqcloud.com/chrome/C03/just_now_tips.png)

这里告诉我们，这个是刚刚执行完代码的结果。

:::tip 敲黑板
`console` 中的对象，在被打印之前是以引用的方式保存的。
:::

### 2.如何正常打印

那如果要打印修改之前的值如何操作？

* 打印一个从这个对象复制出来的对象。
* 使用资源面中的断点来调试
* 使用 `JSON.stringify()` 方法处理打印的结果
* 更多你可以想到的好方法~
