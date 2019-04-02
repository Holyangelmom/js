### slideDown\(\)

##### （1）参考资料

[http://www.runoob.com/jquery/jquery-slide.html](http://www.runoob.com/jquery/jquery-slide.html)

##### （1）定义

jQuery slideDown\(\) 方法用于向下滑动元素。

注意: 要使用 clearTimeout\(\) 方法, 在创建执行定时操作时要使用全局变量：

##### （2）语法

```js
$(selector).slideDown(speed,callback);
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| id\_of\_setinterval | 调用 setTimeout\(\) 函数时所获得的返回值，使用该返回标识符作为参数，可以取消该 setTimeout\(\) 所设定的定时执行操作。 |

##### （3）实例

```js
$("#flip").click(function(){
  $("#panel").slideDown();
});
```



