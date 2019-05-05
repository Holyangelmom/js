### hide\(\)

##### （1）参考资料

[https://www.runoob.com/jquery/eff-hide.html](https://www.runoob.com/jquery/eff-hide.html)

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
| speed | 可选。规定隐藏效果的速度。可能的值：毫秒、"slow"、"fast" |
| easing | 可选。规定在动画的不同点上元素的速度。默认值为 "swing"。可能的值："swing" - 在开头/结尾移动慢，在中间移动快、"linear" - 匀速移动 |
| callback | 可选。hide\(\) 方法执行完之后，要执行的函数。 |

##### （4）实例

```js
$(".btn1").click(function(){
	$("p").hide(1000,function(){
		alert("Hide()方法已完成!");
	});
});
```



