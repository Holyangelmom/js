### hide\(\)

##### （1）参考资料

https://www.runoob.com/jquery/eff-hide.html

##### （2）定义

hide\(\) 方法隐藏被选元素。

提示：这与 CSS 属性 display:none 类似。

注释：隐藏的元素不会被完全显示（不再影响页面的布局）。

##### （3）语法

```js
$(selector).hide(speed,easing,callback)
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| speed | 可选的。规定效果的时长。 |
| callback | 可选的。滑动完成后所执行的函数名称 |

##### （4）实例

```js
$("#flip").click(function(){
    $("#panel").slideDown();
});
```





