# 4.2.6 JS 與 jQuery 操控網頁元素 - 新增

HTML：

```html
<div id="div_block">這是 div 區塊</div>
```

JavaScript：

* **document.createElement\(標籤名稱\)**：建立元素的標籤名稱。
* **{element}.appendChild\(元素\)**：替 {element} 的裡面且最後面，加上新的元素。
* **document.createTextNode\("任何文字"\)**：建立文字節點。



```js
  var para = document.createElement("p");
  var div_block = document.getElementById("div_block");
  div_block.appendChild(para);
  var txt = document.createTextNode("新貼入的文字");
  para.appendChild(txt);
```

結果呈現：

![](/assets/js新增元素.png)

## 完整範例

檔案所在路徑：`js/4.2.6/`。

