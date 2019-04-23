### 7.2.1、前端报错unable to decode value

**问题描述：**

在填写表单时，若存在特殊字符，如：%,$，比如：酒，可能有一个度数这个规格，值为：56%。这个时候，ajax请求传入参数，就会报unable to decode value错误。

**解决办法：**

将字符串用encodeURI函数进行编码，再进行ajax请求，就ok了。

