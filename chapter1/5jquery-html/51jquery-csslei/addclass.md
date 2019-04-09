### addClass\(\)

##### （1）参考资料

[http://www.runoob.com/jquery/html-addclass.html](http://www.runoob.com/jquery/html-addclass.html)

##### （2）定义

addClass\(\) 方法向被选元素添加一个或多个类名。

该方法不会移除已存在的 class 属性，仅仅添加一个或多个类名到 class 属性。

提示：如需添加多个类，请使用空格分隔类名。

##### （3）语法

```js
$(selector).addClass(classname, function(index,oldclass))
```

| **参数** | **描述** |
| :--- | :--- |
| classname | 必需。规定一个或多个要添加的类名称。 |
| function\(index, currentclass\) | 可选。规定返回一个或多个待添加类名的函数。index - 返回集合中元素的 index 位置。currentclass - 返回被选元素的当前类名。 |

##### （4）实例

```js
//向指定元素添加两个类名
$("p:first").addClass("intro note");
```

```js
//使用函数向被选元素添加类
$("p").addClass(function(index, currentclass){
    return "par_" + index;
});
```



