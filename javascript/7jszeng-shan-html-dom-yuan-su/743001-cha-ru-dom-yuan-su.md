### 插入dom元素

##### 1、定义

insertBefore\(\) 方法在您指定的已有子节点之前插入新的子节点。

##### 2、语法

```js
//语法
document.getElementById(id).insertBefore(newItem,existingItem);

//实例
var child = document.createElement("p");
var parent = document.createElement("div");
parent.appendChild(child);
```

##### 3、实例

```js
var newItem=document.createElement("LI")
var textnode=document.createTextNode("Water")
newItem.appendChild(textnode)
var list=document.getElementById("myList")
list.insertBefore(newItem,list.childNodes[0]);
```



