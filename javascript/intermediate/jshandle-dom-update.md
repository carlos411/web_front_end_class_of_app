# 4.2.5 JS 與 jQuery 操控網頁元素 - 更新

HTML：

```html
<p id="the_id">這是段落</p>
```

CSS：

```css
.change_style{
  color: blue;
  font-size: 30px;
}
```

JavaScript：

* **innerHTML**：取得元素的內容。透過「=」，將元素的內容，整個取代。
* **setAttribute\(attribute, value\)**：更新屬性的值。
* **removeAttribute\(attribute\)**：移除屬性。

```js
// 透過 id 取得元素
var para_ele = document.getElementById("the_id");

// 提示訊息出現，得到元素的內容：「這是段落」
alert(para_ele.innerHTML);

// 改變該元素的內容
para_ele.innerHTML = "這是改變的文字";

// 元變元素的某個屬性  
// para_ele.setAttribute("style", "color: red;font-size: 30px;");  
para_ele.setAttribute("class", "change_style");

// 移除元素的屬性  
para_ele.removeAttribute("class");
```

針對 css 類別的新增及移除：

* classList.add\("css 類別名稱"\)
* classList.remove\("css 類別名稱"\)

## 對應的 jQuery 版本：

* **.html\(\)**：取得元素的內容。透過參數代入，將元素的內容，整個取代。
* **.attr\(attribute, value\)**：更新屬性的值。
* **.removeAttr\(attribute\)**：移除屬性。

```js
// 透過 id 取得元素
var para_ele = $("#the_id");

// 提示訊息出現，得到元素的內容：「這是段落」
alert($(para_ele).html());

// 改變該元素的內容
$(para_ele).html("這是改變的文字");

// 元變元素的某個屬性
// $(para_ele).attr("style", "color: red;font-size: 30px;");
$(para_ele).attr("class", "change_style");

// 移除元素的屬性
$(para_ele).removeAttr("class");
```

針對 css 類別的新增及移除：

* addClass\("css 類別名稱"\)
* removeClass\("css 類別名稱"\)

## 練習

開啟以下兩個檔案觀察：

檔案所在路徑：`js/4.2.5/index.html`、`js/4.2.5/index_jquery.html`。

練習 css 類別的新增及移除

```html
<p class="default_style">這是新增的段落</p>
```





