### JQuery选择器

##### 1、参考资料

[http://www.w3school.com.cn/jquery/jquery\_ref\_selectors.asp](http://www.w3school.com.cn/jquery/jquery_ref_selectors.asp)

##### 2、常用选择器

| 选择器 | 实例 | 选取 |
| :--- | :--- | :--- |
| \* | $\("\*"\) | 所有元素 |
| \#id | $\("\#lastname"\) | id="lastname" 的元素 |
| .class | $\(".intro"\) | 所有 class="intro" 的元素 |
| element | $\("p"\) | 所有 &lt;p&gt; 元素 |
| .class.class | $\(".intro.demo"\) | 所有 class="intro" 且 class="demo" 的元素 |
|  |  |  |
| :first | $\("p:first"\) | 第一个 &lt;p&gt; 元素 |
| :last | $\("p:last"\) | 最后一个 &lt;p&gt; 元素 |
| :contains\(text\) | $\(":contains\('W3School'\)"\) | 包含指定字符串的所有元素 |
|  |  |  |
| s1,s2,s3 | $\("th,td,.intro"\) | 所有带有匹配选择的元素 |
| element element | $\("ul li"\) | ul里的所有li |
| element&gt;element | $\("ul&gt;li"\) | ul里的第一个li |
|  |  |  |
| :input | $\(":input"\) | 所有 &lt;input&gt; 元素 |
| :text | $\(":text"\) | 所有 type="text" 的 &lt;input&gt; 元素 |
| :password | $\(":password"\) | 所有 type="password" 的 &lt;input&gt; 元素 |
| :radio | $\(":radio"\) | 所有 type="radio" 的 &lt;input&gt; 元素 |
| :checkbox | $\(":checkbox"\) | 所有 type="checkbox" 的 &lt;input&gt; 元素 |
| :submit | $\(":submit"\) | 所有 type="submit" 的 &lt;input&gt; 元素 |
| :reset | $\(":reset"\) | 所有 type="reset" 的 &lt;input&gt; 元素 |
| :button | $\(":button"\) | 所有 type="button" 的 &lt;input&gt; 元素 |
| :image | $\(":image"\) | 所有 type="image" 的 &lt;input&gt; 元素 |
| :file | $\(":file"\) | 所有 type="file" 的 &lt;input&gt; 元素 |
|  |  |  |
| :enabled | $\(":enabled"\) | 所有激活的 input 元素 |
| :disabled | $\(":disabled"\) | 所有禁用的 input 元素 |
| :selected | $\(":selected"\) | 所有被选取的 input 元素 |
| :checked | $\(":checked"\) | 所有被选中的 input 元素 |

##### 3、实例

##### （1）基本选择器

$\("\#id"\)            //ID选择器

$\("div"\)            //元素选择器

$\(".classname"\)     //类选择器

$\(".classname,.classname1,\#id1"\)     //组合选择器

##### （2）层次选择器

 $\("\#id&gt;.classname "\)    //子元素选择器

$\("\#id .classname "\)    //后代元素选择器

$\("\#id + .classname "\)    //紧邻下一个元素选择器

$\("\#id ~ .classname "\)    //兄弟元素选择器

##### （3）过滤选择器\(重点\)

$\("li:first"\)    //第一个li

$\("li:last"\)     //最后一个li

$\("li:even"\)     //挑选下标为偶数的li

$\("li:odd"\)      //挑选下标为奇数的li

$\("li:eq\(4\)"\)    //下标等于 4 的li\(第五个 li 元素\)

$\("li:gt\(2\)"\)    //下标大于 2 的li

$\("li:lt\(2\)"\)    //下标小于 2 的li

$\("li:not\(\#runoob\)"\) //挑选除 id="runoob" 以外的所有li

##### （4）内容过滤选择器

$\("div:contains\('Runob'\)"\)    // 包含 Runob文本的元素

$\("td:empty"\)                 //不包含子元素或者文本的空元素

$\("div:has\(selector\)"\)        //含有选择器所匹配的元素

$\("td:parent"\)                //含有子元素或者文本的元素

##### （5）可见性过滤选择器

$\("li:hidden"\)       //匹配所有不可见元素，或type为hidden的元素

$\("li:visible"\)      //匹配所有可见元素

##### （6）属性过滤选择器

$\("div\[id\]"\)        //所有含有 id 属性的 div 元素

$\("div\[id='123'\]"\)        // id属性值为123的div 元素

$\("div\[id!='123'\]"\)        // id属性值不等于123的div 元素

$\("div\[id^='qq'\]"\)        // id属性值以qq开头的div 元素

$\("div\[id$='zz'\]"\)        // id属性值以zz结尾的div 元素

$\("div\[id\*='bb'\]"\)        // id属性值包含bb的div 元素

$\("input\[id\]\[name$='man'\]"\) //多属性选过滤，同时满足两个属性的条件的元素

##### （7）状态过滤选择器

$\("input:enabled"\)    // 匹配可用的 input

$\("input:disabled"\)   // 匹配不可用的 input

$\("input:checked"\)    // 匹配选中的 input

$\("option:selected"\)  // 匹配选中的 option

##### （8）表单选择器

$\(":input"\)      //匹配所有 input, textarea, select 和 button 元素

$\(":text"\)       //所有的单行文本框，$\(":text"\) 等价于$\("\[type=text\]"\)，推荐使用$\("input:text"\)效率更高，下同

$\(":password"\)   //所有密码框

$\(":radio"\)      //所有单选按钮

$\(":checkbox"\)   //所有复选框

$\(":submit"\)     //所有提交按钮

$\(":reset"\)      //所有重置按钮

$\(":button"\)     //所有button按钮

$\(":file"\)       //所有文件域

