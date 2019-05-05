### 9、JQuery事件监听方法

##### （1）bind

bind\(type,\[data\],function\(eventObject\)\)  bind是使用频率较高的一种，作用就是在选择到的元素上绑定特定事件类型的监听函数，

参数如下：

* type:事件类型，如click、change、mouseover等；
* data:传入监听函数的参数，通过event.data取到；
* function:监听函数，可传入event对象，这里的event是jquery封装的event对象。

源码：

```js
//可以看到内部是调用了on方法。
bind: function( types, data, fn ) {
    return this.on( types, null, data, fn );
}
```

实例：

```
$('div').bind('click',function(){    
    if($(this).text()=='列表4'){
        $(this).after('<div>列表5</div>');
    }
    alert($(this).text());
})
```



