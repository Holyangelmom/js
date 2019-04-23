### 获取dom元素

##### 1、getElementById

```js
//语法
document.getElementById(id);
//返回值
返回相同id的dom对象中的第一个，按在页面中出现的次序,如果无符合条件的对象，则返回 null

//实例
var div = document.getElementById("div1");
```

##### 2、document.getElementsByName\(name\)

```js
//语法
document.getElementsByName(name)
//返回值
数组对象; 如果无符合条件的对象，则返回空数组，按在页面中出现的次序


//实例
var value = document.getElementsByName("name1")[0].value;
```

##### 3、getElementsByTagName

```js
//语法
document.getElementsByTagName(tagName)
//返回值
返回值：数组对象; 如果无符合条件的对象，则返回空数组，按在页面中出现的次序


//实例
var value = document.getElementsByTagName("p")[0].childNodes[0].nodeValue;
```

##### 4、getElementsByClassName\(\)

```js
//语法
document.getElementsByClassName(className);
//返回值
返回值：数组对象; 如果无符合条件的对象，则返回空数组，按在页面中出现的次序


//实例
var value = document.getElementsByClassName("className")[0].childNodes[0].nodeValue;
```



