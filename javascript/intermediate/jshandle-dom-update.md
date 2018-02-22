# 4.2.5 JS 與 jQuery 操控網頁元素 - 更新

HTML

```html
<p id="the_id">這是段落</p>
```

JavaScript

* innerHTML：將元素的內容，整個取代。
* setAttribute\(attribute, value\)：更新屬性的值。

* removeAttribute\(attribute\)：移除屬性。

```js
// 改變該元素的內容
para_ele.innerHTML = "這是改變的文字";

// 元變元素的某個屬性  
// para_ele.setAttribute("style", "color: red;font-size: 30px;");  
para_ele.setAttribute("class", "change_style");

// 移除元素的屬性  
para_ele.removeAttribute("class");
```



