### 9、JQuery事件监听方法

##### （1）bind

bind是使用频率较高的一种，作用就是在选择到的元素上绑定特定事件类型的监听函数。

语法：

```js
bind(type,[data],function(eventObject))
```

参数：

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

```js
$('div').bind('click',function(){    
    if($(this).text()=='列表4'){
        $(this).after('<div>列表5</div>');
    }
    alert($(this).text());
})
```

##### （2）on

语法：

```js
on(type,[selector],[data],fn)
```

参数：

* type：事件类型，如click、change、mouseover等；
* selector：可选，被选元素及子元素；
* data：可选，通过event.data取到；
* function：监听函数，可传入event对象，这里的event是jquery封装的event对象。

on\(\) 方法在被选元素及子元素上添加一个或多个事件处理程序。

自 jQuery 版本 1.7 起，on\(\) 方法是 bind\(\)、live\(\) 和 delegate\(\) 方法的新的替代品。

代码，实现效果同上，把delegate改为on，第一个参数为click，第二个参数p可写可不写，第三个参数同上。

```
$\(function\(\){

        $\('div'\).on\('click','p',function\(\){    

            $\('p'\).css\('color','red'\);    

        }\);
```



