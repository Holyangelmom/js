### removeClass\(\)

##### （1）参考资料

[http://www.runoob.com/jquery/html-removeclass.html](http://www.runoob.com/jquery/html-removeclass.html)

##### （2）定义

removeClass\(\) 方法从被选元素移除一个或多个类。

注意：如果没有规定参数，则该方法将从被选元素中删除所有类。

##### （3）语法

```js
$(selector).removeClass(classname, function(index,currentclass))
```

| **参数** | **描述** |
| :--- | :--- |
| classname | 可选。规定要移除的一个或多个类名称。如需移除若干个类，请使用空格分隔类名称。注意： 如果该参数为空，则将移除所有类名称。 |
| function\(index, currentclass\) | 可选。返回要移除的一个或多个类名称的函数。index - 返回集合中元素的 index 位置。currentclass - 返回被选元素的当前类名。 |

（4）实例

```js
//从被选元素移除若干个类名。
$("p,h1").removeClass("head intro main");
```



