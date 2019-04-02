### slideToggle\(\)

##### （1）参考资料

[http://www.runoob.com/jquery/jquery-slide.html](http://www.runoob.com/jquery/jquery-slide.html)

##### （1）定义

jQuery slideToggle\(\) 方法可以在 slideDown\(\) 与 slideUp\(\) 方法之间进行切换。

如果元素向下滑动，则 slideToggle\(\) 可向上滑动它们。

如果元素向上滑动，则 slideToggle\(\) 可向下滑动它们。

##### （2）语法

```js
$(selector).slideToggle(speed,callback);
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| speed | 可选的。规定效果的时长。 |
| callback | 可选的。滑动完成后所执行的函数名称 |

##### （3）实例

```js
$("#flip").click(function(){
    $("#panel").slideToggle();
});
```



