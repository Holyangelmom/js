### 8、比较两个日期的大小的2种方法

（1）转换为date对象进行比较操作

注意：因为IE不支持

```js
var st="2009-10-20 14:38:40"
var et="2009-10-20 15:38:40"
var stdt=new Date(st.replace("-","/"));
var etdt=new Date(et.replace("-","/"));
if(stdt>etdt) alert("开始时间必须小于结束时间")
```

（2）直接比较大小即可

```js
var st="2009-10-20 14:38:40"
var et="2009-10-20 15:38:40"
if(st>et) alert("开始时间必须小于结束时间")
```



