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

等价于

* $.fn.extend\(object\);
* $.extend\(object\);

##### （5）第一种开发方式

JQuery.fn.extend\(object\);

$.fn.extend\(object\);

```js
;(function($) {


}(jQuery));
```



