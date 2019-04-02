### 1.2、参数扩展

JQuery参数也可以扩展。依据两种插件扩展方式，参数扩展也有两种。

##### （1）第一种方式

```js
;(function($){
    $.fn.函数名 = function(options) {  
        var defaults = {  
            foreground: 'red',  
            background: 'yellow'  
        };  
        var opts = $.extend(defaults, options);
    };
})(jQuery);
```

##### （2）第二种方式

```js
;(function($){
    $.fn.extend({
        "函数名":function(options){
            options = $.extend({
                foreground:'red',
                background:'yellow'
            },options);
        }
    });
})(jQuery);
```

##### （3）调用



