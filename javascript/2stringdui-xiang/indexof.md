### indexOf\(\)

##### （1）参考资料

[http://www.w3school.com.cn/jsref/jsref\_indexOf.asp](http://www.w3school.com.cn/jsref/jsref_indexOf.asp)

##### （2）定义

indexOf\(\) 方法可返回某个指定的字符串值在字符串中首次出现的位置。如果要检索的字符串值没有出现，则该方法返回 -1。indexOf\(\) 方法对大小写敏感！

##### （3）语法

```js
stringObject.indexOf(searchvalue,fromindex)
```

| 参数 | 描述 |
| :--- | :--- |
| searchvalue | 必需。规定需检索的字符串值。 |
| fromindex | 可选的整数参数。规定在字符串中开始检索的位置。它的合法取值是 0 到 stringObject.length - 1。如省略该参数，则将从字符串的首字符开始检索。 |

##### （4）实例

```js
var str1="Hello "
var str2="world!"
document.write(str1.concat(str2))
```



