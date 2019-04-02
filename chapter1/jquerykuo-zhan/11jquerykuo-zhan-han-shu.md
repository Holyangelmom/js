### 1.1、函数扩展

在《1、JQuery扩展》中讲到，JQuery为开发插件的两个方法。下面讲解这两种方式。

##### （1）第一种开发方式

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

##### （2）第二种开发方式

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



