# 3.5 區塊模型\(Box Model\)

**margin**：border 往外的距離。

**padding**：內容與 border 的距離。

**border**：該元素的邊框。

## 範例

第一步：增加 **border**。

HTML：

```html
<span class="span1">這是文字1</span>
```

CSS：

```css
.span1{
  /* 1px 的框線、實線、紅色 */
  border:1px solid red;
}
```

![](/assets/box_model_example.png)

第二步：增加 **padding**。

更改 CSS 如下：

```css
.span1{
  /* 1px 的框線、實線、紅色 */
  border:1px solid red;

  /* 內容與框線的上、右、下、左，距離都是 10px */
  padding: 10px;
}
```

![](/assets/box_model_example2.png)

第三步：增加 **margin**。

更改 css 如下：

```css
.span1{
  /* 1px 的框線、實線、紅色 */
  border:1px solid red;

  /* 內容與框線的上、右、下、左，距離都是 10px */
  padding: 10px;

  /* 框線與上、右、下、左，距離都是 20px */
  margin: 20px;
}
```

![](/assets/box_model_example3.png)



## 行內元素、區塊元素、行內區塊元素



註1：上下 margin 相鄰時，會合併，並取最大的。

註2：inline 元素，上下並不會產生 margin。

