### replace\(\)

##### （1）参考资料

[http://www.w3school.com.cn/jsref/jsref\_replace.asp](http://www.w3school.com.cn/jsref/jsref_replace.asp)

##### （2）定义

replace\(\) 方法用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串。

注意： match\(\) 方法将检索字符串 String Object，以找到一个或多个与 regexp 匹配的文本。这个方法的行为在很大程度上有赖于 regexp 是否具有标志 g。如果 regexp 没有标志 g，那么 match\(\) 方法就只能在 stringObject 中执行一次匹配。如果没有找到任何匹配的文本， match\(\) 将返回 null。否则，它将返回一个数组，其中存放了与它找到的匹配文本有关的信息。

##### （3）语法

```js
stringObject.replace(regexp/substr,replacement)
```

| 参数 | 描述 |
| :--- | :--- |
| regexp/substr | 必需。规定子字符串或要替换的模式的 RegExp 对象。请注意，如果该值是一个字符串，则将它作为要检索的直接量文本模式，而不是首先被转换为 RegExp 对象。 |
| replacement | 必需。一个字符串值。规定了替换文本或生成替换文本的函数。 |

返回值

| 类型 | 描述 |
| :--- | :--- |
| String | 一个新的字符串，是用 replacement 替换了 regexp 的第一次匹配或所有匹配之后得到的。 |

##### 说明

字符串 stringObject 的 replace\(\) 方法执行的是查找并替换的操作。它将在 stringObject 中查找与 regexp 相匹配的子字符串，然后用 replacement 来替换这些子串。如果 regexp 具有全局标志 g，那么 replace\(\) 方法将替换所有匹配的子串。否则，它只替换第一个匹配子串。

replacement 可以是字符串，也可以是函数。如果它是字符串，那么每个匹配都将由字符串替换。但是 replacement 中的 $ 字符具有特定的含义（类似于notepad++的查找替换）。如下表所示，它说明从模式匹配得到的字符串将用于替换。

| 字符 | 替换文本 |
| :--- | :--- |
| $1、$2、...、$99 | 与 regexp 中的第 1 到第 99 个子表达式相匹配的文本。 |
| $& | 与 regexp 相匹配的子串。 |
| $\` | 位于匹配子串左侧的文本。 |
| $' | 位于匹配子串右侧的文本。 |
| $$ | 直接量符号。 |

##### （4）实例

```js
//使用 "W3School" 替换字符串中的 "Microsoft"：
var str="Visit Microsoft!"
document.write(str.replace(/Microsoft/, "W3School"))


//输出：
Visit W3School!
```

```js
//执行一次全局替换，每当 "Microsoft" 被找到，它就被替换为 "W3School"：


var str="Welcome to Microsoft! "
str=str + "We are proud to announce that Microsoft has "
str=str + "one of the largest Web Developers sites in the world."

document.write(str.replace(/Microsoft/g, "W3School"))

//输出：
Welcome to W3School! We are proud to announce that W3School
has one of the largest Web Developers sites in the world.
```

```js
//执行一个全局替换, 忽略大小写:
var str="Mr Blue has a blue house and a blue car";
var n=str.replace(/blue/gi, "red");
//n 输出结果:
Mr red has a red house and a red car
```



