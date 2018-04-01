# 3.19 overflow

當內容超出元素區域的，用來定義該如何處理超出的內容。常見可選的值有：

* `visible`：這是預設值，即正常出現。

## 範例

html

```html
<div class="test_div">這是 div 的內容這是 div 的內容這是 div 的內容這是 div 的內容這是 div 的內容</div>
```

css

```css
div.test_div{
  border:2px solid red;
  width: 100px;
  height: 100px;
}
```

結果如圖：

![](/assets/overflow_1.png)

css 改成…

```css
div.test_div{
  border:2px solid red;
  width: 100px;
  height: 100px;
  overflow: hidden;
}
```

結果如圖：

![](/assets/overflow_2.png)

