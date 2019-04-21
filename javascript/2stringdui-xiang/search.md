### search\(\)

##### （1）参考资料

http://www.w3school.com.cn/jsref/jsref\_search.asp

##### （2）定义

search\(\) 方法用于检索字符串中指定的子字符串，或检索与正则表达式相匹配的子字符串。

search\(\) 方法不执行全局匹配，它将忽略标志 g。它同时忽略 regexp 的 lastIndex 属性，并且总是从字符串的开始进行检索，这意味着它总是返回 stringObject 的第一个匹配的位置。

##### （3）语法

```js
stringObject.search(regexp)
```

| 参数 | 描述 |
| :--- | :--- |
| regexp | 该参数可以是需要在 stringObject 中检索的子串，也可以是需要检索的 RegExp 对象。注释：要执行忽略大小写的检索，请追加标志 i。 |

返回值

stringObject 中第一个与 regexp 相匹配的子串的起始位置。如果没有找到任何匹配的子串，则返回 -1。

##### （4）实例

```js
//执行一次忽略大小写的检索：

var str="Visit W3School!"
document.write(str.search(/w3school/i))

//输出：
6
```



