# 4.2.6 JS 與 jQuery 操控網頁元素 - 新增

JavaScript

```js
var para = document.createElement("p");
var div_block = document.getElementById("div_block");
div_block.appendChild(para);
var txt = document.createTextNode("新貼入的文字");
para.appendChild(txt);
```



