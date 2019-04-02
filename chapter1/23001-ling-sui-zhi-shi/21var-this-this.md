### 2.1、var $this = $\(this\)

##### （1）参考资料

https://blog.csdn.net/mxt123456/article/details/53152398/

##### （2）解释

在jquery插件文件中常看到这句代码，但不知是啥意思。那它究竟啥意思？有何作用？

**含义：**

 this其实是一个html 元素。 

$this 只是个变量名，加$是为说明其是个jquery对象。 

而$\(this\)是个转换，将this表示的dom对象转为jquery对象，这样就可以使用jquery提供的方法操作。

**作用：**

把当前对象保存起来，便于后边的使用。

