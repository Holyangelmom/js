### toggle\(\)

##### （1）参考资料

https://www.runoob.com/jquery/eff-toggle.html

##### （2）定义

toggle\(\) 方法在被选元素上进行 hide\(\) 和 show\(\) 之间的切换。

该方法检查被选元素的可见状态。如果一个元素是隐藏的，则运行 show\(\)，如果一个元素是可见的，则运行 hide\(\) - 这会造成一种切换的效果。

注释：隐藏的元素不会被完全显示（不再影响页面的布局）。

##### （3）语法

```js
$(selector).toggle(speed,easing,callback)
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| speed | 可选。规定隐藏效果的速度。可能的值：毫秒、"slow"、"fast" |
| easing | 可选。规定在动画的不同点上元素的速度。默认值为 "swing"。可能的值："swing" - 在开头/结尾移动慢，在中间移动快、"linear" - 匀速移动 |
| callback | 可选。toggle\(\) 方法执行完之后，要执行的函数。 |

##### （4）实例

```js
$("button").click(function(){
	$("p").toggle(1000,function(){
		alert("toggle() 方法已完成!");
	});
});
```



