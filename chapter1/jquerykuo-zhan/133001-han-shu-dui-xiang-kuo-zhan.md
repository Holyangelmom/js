### 1.3、函数对象扩展

JQuery函数对象也可以扩展。依据两种插件扩展方式，函数对象扩展也有两种。

（1）第一种方式

```js
;(function($){
    $.fn.函数名 = function(options) {  
        var opts = $.extend({}, , options);
    };
    
    $.fn.函数名.defaults = {
        color: 'red',
        background: 'yellow'
    };
})(jQuery);
```



