### false、0、空字符串、null和undefined

##### 1、划分

false、0、空字符串、null、undefined被划分为两类：假值、空值。0、空字符串和false归为一类，称为“假值”；把null和undefined归为一类，称为“空值”。假值还算一个有效的对象，因此可以对其使用toString等类型相关的方法，而空值则将会抛出异常：xxx hash no properties。

##### 2、假值和空值作为if条件分支

这是工作期间经常遇到的问题，总分不清这些值为true还是false。其实假值和空值有一个共性，那就是在作为if的条件分支时，均被视为false；应用“!”操作之后得到的均为true。

这五个值作!运算，结果全为：true  

* alert\(!0\); //true  
* alert\(!false\); //true  
* alert\(!undefined\); //true  
* alert\(!null\); //true  
* alert\(!''\); //true  



