# 3.5 區塊模型\(Box Model\)

margin：border 往外的距離。

padding：內容與 border 的距離。

border：該視素的邊框。

![](/assets/box_model.png)

註：上下 margin 相鄰時，會合併，並取最大的。

## 範例 1

HTML：

```html
<span class="span1">這是文字1</span>
```

CSS：

```css
.span1{
  border:1px solid red;
}
```

![](/assets/box_model_example.png)

