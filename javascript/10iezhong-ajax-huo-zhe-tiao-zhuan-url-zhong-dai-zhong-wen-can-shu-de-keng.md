### 10、IE中ajax或者跳转url中带中文参数的坑

ie中url 是不支持中文，需要将中文转码（ajax中的url含中文参数也是要encode\(url\)）。

页面跳转的时候对url进行encodeURI转码，到其他页面再进行decodeURI转码



