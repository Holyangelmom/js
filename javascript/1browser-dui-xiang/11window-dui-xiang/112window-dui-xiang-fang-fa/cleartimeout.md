### clearTimeout\(\)

##### （1）参考资料

[http://www.runoob.com/jsref/met-win-settimeout.html](http://www.runoob.com/jsref/met-win-settimeout.html)

##### （1）定义

setTimeout\(\) 方法用于在指定的毫秒数后调用函数或计算表达式。使用 clearTimeout\(\) 方法来阻止函数的执行。

##### （2）语法

```
setTimeout(code, milliseconds, param1, param2, ...)
setTimeout(function, milliseconds, param1, param2, ...)
```

参数：

| 参数 | 描述 |
| :--- | :--- |
| code/function | 必需。要调用一个代码串，也可以是一个函数。 |
| milliseconds | 可选。执行或调用 code/function 需要等待的时间，以毫秒计。默认为 0。 |
| param1, param2, ... | 可选。 传给执行函数的其他参数（IE9 及其更早版本不支持该参数）。 |

返回值：

| 返回值 | 返回一个 ID（数字），可以将这个ID传递给 clearTimeout\(\) 来取消执行。 |
| :--- | :--- |


##### （3）实例

```js
var myVar;
myVar = setTimeout(function(){alert("Hello") }, 3000);
clearTimeout(myVar);
```



