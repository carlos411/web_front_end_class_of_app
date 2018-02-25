# 4.2.7 JS 與 jQuery 操控網頁元素 - 刪除

HTML：

```html
<div id="div_block_1">這是第一個 div 區塊</div>
<div id="div_block_2">這是第二個 div 區塊</div>
```

JavaScript：

```js
// 取得 id 為 div_block_1 的元素，並存於 div_block_1 變數之中
var div_block_1 = document.getElementById("div_block_1");
div_block_1.remove();
```

## 完整範例

檔案所在路徑：`js/4.2.7/`。

