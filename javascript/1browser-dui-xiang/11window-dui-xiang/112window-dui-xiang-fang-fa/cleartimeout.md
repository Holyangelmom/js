### clearTimeout\(\)

##### （1）参考资料

[http://www.runoob.com/jsref/met-win-cleartimeout.html](http://www.runoob.com/jsref/met-win-cleartimeout.html)

##### （2）定义

clearTimeout\(\) 方法可取消由 setTimeout\(\) 方法设置的定时操作。

clearTimeout\(\) 方法的参数必须是由 setTimeout\(\) 返回的 ID 值。

注意: 要使用 clearTimeout\(\) 方法, 在创建执行定时操作时要使用全局变量：

##### （3）语法

```
clearTimeout(id_of_settimeout)
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| id\_of\_setinterval | 调用 setTimeout\(\) 函数时所获得的返回值，使用该返回标识符作为参数，可以取消该 setTimeout\(\) 所设定的定时执行操作。 |

##### （4）实例

```js
var myVar;
//匿名函数，所有函数都支持
myVar = setTimeout(function(){alert("Hello") }, 3000);
clearTimeout(myVar);
```



