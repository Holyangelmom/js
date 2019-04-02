### slideUp\(\)

##### （1）参考资料

[http://www.runoob.com/jquery/jquery-slide.html](http://www.runoob.com/jquery/jquery-slide.html)

##### （1）定义

jQuery slideUp\(\) 方法用于向上滑动元素。

##### （2）语法

```js
$(selector).slideUp(speed,callback);
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| speed | 可选的。规定效果的时长。 |
| callback | 可选的。滑动完成后所执行的函数名称 |

##### （3）实例

```js
$("#flip").click(function(){
    $("#panel").slideDown();
});
```



