# 4.2.6 JS 與 jQuery 操控網頁元素 - 新增

HTML：

```html
<div id="div_block">這是 div 區塊</div>
```

JavaScript：

```js
var para = document.createElement("p");
var div_block = document.getElementById("div_block");
div_block.appendChild(para);
var txt = document.createTextNode("新貼入的文字");
para.appendChild(txt);
```



