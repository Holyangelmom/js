### 1、JQuery扩展

##### （1）参考资料

[https://blog.csdn.net/ruru7989/article/details/79939924](https://blog.csdn.net/ruru7989/article/details/79939924)

#### （2）前言

项目开发时，经常需要看看js源代码。奈何菜鸡难啄巨米，呛着难受。鉴于已经多次出现类似情况，所以还得静下心来磨一磨鸡嘴。

##### （3）创建闭包

JQuery扩展插件都需要创建闭包，扩展代码都在闭包当中。闭包代码规范如下：

```js
;(function($) {


}(jQuery));
```

##### （4）两种插件开发方式

JQuery为开发插件的两个方法：

* JQuery.fn.extend\(object\);
* JQuery.extend\(object\);

等价于：

* $.fn.extend\(object\);
* $.extend\(object\);

两种开发方式对比：

* 代码形式上有没有fn
* jQuery.fn.extend\(object\) 给jQuery对象添加方法；jQuery.extend\(object\) 为扩展jQuery类本身.为类添加新的方法，可以理解为添加静态方法。

##### （5）第一种开发方式

JQuery.fn.extend\(object\);

$.fn.extend\(object\);

代码规范：

```js
;(function($) {
    $.fn.extend({
        "函数名":function(自定义参数){

        }
    });
}(jQuery));

//或者

;(function($) {
    $.fn.函数名=function(自定义参数){

    }
}(jQuery));
```

调用方式：

```js
$("#id").函数名(参数)
```

##### （5）第二种开发方式

JQuery.extend\(object\);

$.extend\(object\);

代码规范：

```js
;(function($) {
   $.extend({
        "函数名":function(自定义参数){

    }
    });
}(jQuery));

//或者

;(function($) {
    $.函数名=function(自定义参数){


    }
}(jQuery));
```

调用方式：

```js
$.函数名(参数) 或 jQuery.函数名(参数);
```



