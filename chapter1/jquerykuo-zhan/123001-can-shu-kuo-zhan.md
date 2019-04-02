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

编写插件

```js
;(function($) {
    // plugin definition
    $.fn.hilight = function(options) {
        var defaults = {
            color : 'red',
            background : 'yellow'
        };

        var opts = $.extend(defaults, options);

        var $this = $(this);
        //调用jquery方法css();
        $this.css({
            background : opts.background,
            color : opts.color
        })
    };
})(jQuery);
```

调用

```js
    // 使用默认值
    $('#link_tilte_a').hilight();

    // 改变默认值
    $('#link_tilte_a').hilight({
        "color" : "pink"
    });

    //单独定义一个变量传入
    var dataInit = {
        "color" : "pink",
        "background" : "red"
    };
    $('#link_tilte_a').hilight(dataInit);
```



