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
	  // Extend our default options with those provided.  
	  var opts = $.extend(defaults, options);  
	  // Our plugin implementation code goes here.  
	};
})(jQuery);
```



