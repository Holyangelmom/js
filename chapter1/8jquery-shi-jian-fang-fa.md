### 8、jQuery 事件方法

##### （1）参考资料

[https://www.runoob.com/jquery/jquery-ref-events.html](https://www.runoob.com/jquery/jquery-ref-events.html)

##### （2）事件方法列表

事件方法触发器或添加一个函数到被选元素的事件处理程序。  
下面的表格列出了所有用于处理事件的 jQuery 方法。

| 方法 | 描述 |
| :--- | :--- |
| [bind\(\)](https://www.runoob.com/jquery/event-bind.html) | 向元素添加事件处理程序 |
| [blur\(\)](https://www.runoob.com/jquery/event-blur.html) | 添加/触发失去焦点事件 |
| [change\(\)](https://www.runoob.com/jquery/event-change.html) | 添加/触发 change 事件 |
| [click\(\)](https://www.runoob.com/jquery/event-click.html) | 添加/触发 click 事件 |
| [dblclick\(\)](https://www.runoob.com/jquery/event-dblclick.html) | 添加/触发 double click 事件 |
| [focus\(\)](https://www.runoob.com/jquery/event-focus.html) | 添加/触发 focus 事件 |
| [focusin\(\)](https://www.runoob.com/jquery/event-focusin.html) | 添加事件处理程序到 focusin 事件 |
| [focusout\(\)](https://www.runoob.com/jquery/event-focusout.html) | 添加事件处理程序到 focusout 事件 |
| [hover\(\)](https://www.runoob.com/jquery/event-hover.html) | 添加两个事件处理程序到 hover 事件 |
| [keydown\(\)](https://www.runoob.com/jquery/event-keydown.html) | 添加/触发 keydown 事件 |
| [keypress\(\)](https://www.runoob.com/jquery/event-keypress.html) | 添加/触发 keypress 事件 |
| [keyup\(\)](https://www.runoob.com/jquery/event-keyup.html) | 添加/触发 keyup 事件 |
| [mousedown\(\)](https://www.runoob.com/jquery/event-mousedown.html) | 添加/触发 mousedown 事件 |
| [mouseenter\(\)](https://www.runoob.com/jquery/event-mouseenter.html) | 添加/触发 mouseenter 事件 |
| [mouseleave\(\)](https://www.runoob.com/jquery/event-mouseleave.html) | 添加/触发 mouseleave 事件 |
| [mousemove\(\)](https://www.runoob.com/jquery/event-mousemove.html) | 添加/触发 mousemove 事件 |
| [mouseout\(\)](https://www.runoob.com/jquery/event-mouseout.html) | 添加/触发 mouseout 事件 |
| [mouseover\(\)](https://www.runoob.com/jquery/event-mouseover.html) | 添加/触发 mouseover 事件 |
| [mouseup\(\)](https://www.runoob.com/jquery/event-mouseup.html) | 添加/触发 mouseup 事件 |
| [off\(\)](https://www.runoob.com/jquery/event-off.html) | 移除通过 on\(\) 方法添加的事件处理程序 |
| [on\(\)](https://www.runoob.com/jquery/event-on.html) | 向元素添加事件处理程序 |
| [one\(\)](https://www.runoob.com/jquery/event-one.html) | 向被选元素添加一个或多个事件处理程序。该处理程序只能被每个元素触发一次 |
| [ready\(\)](https://www.runoob.com/jquery/event-ready.html) | 规定当 DOM 完全加载时要执行的函数 |
| [resize\(\)](https://www.runoob.com/jquery/event-resize.html) | 添加/触发 resize 事件 |
| [scroll\(\)](https://www.runoob.com/jquery/event-scroll.html) | 添加/触发 scroll 事件 |
| [select\(\)](https://www.runoob.com/jquery/event-select.html) | 添加/触发 select 事件 |
| [submit\(\)](https://www.runoob.com/jquery/event-submit.html) | 添加/触发 submit 事件 |

##### （3）实例

对于由 jQuery 动态生成的元素，如用 jQuery 给元素添加 class，或者直接添加一对 p 标签，不能直接绑定常用的事件，如 click。因为这些元素属于动态生成，除非采用 noclick 内联的形式。那么解决办法是使用 live 和 on 事件方法。

注意，jquery 1.7.2 之后的版本不建议使用 live。

```js
//例如：
$(".box ").click(function(){});

//类名为 box 的元素是由 jquery 动态生成，以上写法将会无效，那么可以改为如下：
$(".box ").live('click', function(){});

//或者：
$(".box ").on('click', function(){});
```



