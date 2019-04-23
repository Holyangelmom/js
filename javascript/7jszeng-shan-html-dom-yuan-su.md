### js操作html dom元素

##### 1、获取dom元素

```js
//语法
document.getElementById(id);
//返回值
返回相同id的dom对象中的第一个，按在页面中出现的次序,如果无符合条件的对象，则返回 null

//实例
var div= document.getElementById("div1");
```

##### 2、创建dom元素

```js
//语法
document.createElement(domElementName);


//实例
var p = document.createElement("p");
var div = document.createElement("div");
var form = document.createElement("form");
```

3、

