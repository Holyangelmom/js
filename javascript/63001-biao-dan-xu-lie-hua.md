### 表单序列化

| 函数 | 语法 | 描述 |
| :--- | :--- | :--- |
| serialize\(\) | $\(selector\).serialize\(\) | serialize\(\) 方法通过序列化表单值，创建 URL 编码文本字符串。可以选择一个或多个表单元素（比如 input 及/或 文本框），或者 form 元素本身。序列化的值可在生成 AJAX 请求时用于 URL 查询字符串中。 |
| serializeArray\(\) | $\(selector\).serializeArray\(\) | serializeArray\(\) 方法序列化表单元素（类似 .serialize\(\) 方法），返回 JSON 数据结构数据。注意：此方法返回的是 JSON 对象而非 JSON 字符串。返回的 JSON 对象是由一个对象数组组成的，其中每个对象包含一个或两个名值对 —— name 参数和 value 参数（如果 value 不为空的话）。 |

实例

```js
$('form').submit(function() {
  alert($(this).serialize());
  return false;
});
//输出标准的查询字符串：
a=1&b=2&c=3&d=4&e=5
```

```js
$("form").submit(function() {
    console.log($(this).serializeArray());
    return false;
});
//上面的代码产生下面的数据结构（假设浏览器支持 console.log）：
[
  {
    name: a
    value: 1
  },
  {
    name: b
    value: 2
  },
  {
    name: c
    value: 3
  },
  {
    name: d
    value: 4
  },
  {
    name: e
    value: 5
  }
]
```



