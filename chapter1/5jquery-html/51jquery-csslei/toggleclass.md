### toggleClass\(\)

##### （1）参考资料

[http://www.runoob.com/jquery/html-toggleclass.html](http://www.runoob.com/jquery/html-toggleclass.html)

##### （2）定义

toggleClass\(\) 方法对添加和移除被选元素的一个或多个类进行切换。

该方法检查每个元素中指定的类。如果不存在则添加类，如果已设置则删除之。这就是所谓的切换效果。

然而，通过使用 "switch" 参数，您能够规定只删除或只添加类。

##### （3）语法

```js
$(selector).toggleClass(classname,function(index,currentclass),switch)
```

| **参数** | **描述** |
| :--- | :--- |
| classname | 必需。规定添加或移除的一个或多个类名。如需规定若干个类，请使用空格分隔类名。 |
| function\(index, currentclass\) | 可选。返回要移除的一个或多个类名称的函数。index - 返回集合中元素的 index 位置。currentclass - 返回被选元素的当前类名。 |
| switch | 可选。布尔值，规定是否仅仅添加（true）或移除（false）类。 |

（4）实例

```js
//使用 toggleClass() 方法来对添加和移除类进行切换
$("p").toggleClass("main");
```

```js
//使用函数来规定当前元素需切换哪个类名。
$("li").toggleClass(function(n, currentclass){
    return "listitem_" + n;
});
```

```js
//使用 switch 参数来仅仅添加或移除类名。
$("p").toggleClass("main",false);
```



