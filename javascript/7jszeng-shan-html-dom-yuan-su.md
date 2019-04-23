### js操作html dom元素

##### 

##### 2、创建dom元素

```js
//语法
document.createElement(domElementName);


//实例
var p = document.createElement("p");
var div = document.createElement("div");
var form = document.createElement("form");
```

##### 3、追加dom元素

```js
//语法
parentElement.appendChild(childElement);

//实例
var child = document.createElement("p");
var parent = document.createElement("div");
parent.appendChild(child);
```

4、插入元素

