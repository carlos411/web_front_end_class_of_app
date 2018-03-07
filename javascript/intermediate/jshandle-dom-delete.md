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

// 將 div_block_1 元素移除
div_block_1.remove();
```

結果呈現：

![](/assets/js移除元素.png)

對應的 jQuery 版本：

```js
// 取得 id 為 div_block_1 的元素，並存於 div_block_1 變數之中
var div_block_1 = $("#div_block_1");

// 將 div_block_1 元素移除
$(div_block_1).remove();
```

## 練習

開啟以下兩個檔案觀察：

檔案所在路徑：`js/4.2.7/index.html`、`js/4.2.7/index_jquery.html`。

