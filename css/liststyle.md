# 3.8 列表樣式

無序列表結構：

```html
<ul class="unorder_list">
  <li></li>
  <li></li>
</ul>
```

有序列表結構：

```html
<ol class="order_list">
  <li></li>
  <li></li>
</ol>
```

上面 html 的呈現結果：試著觀察預設的列表樣式。

![](/assets/list_basic_style.png)

## 列表相關 CSS 樣式

`list-style`：可選的常用值有 **circle**、**decimal**、**none**、**inside**、**lower-alpha**、**lower-roman**、**square**、**lower-alpha**、**lower-roman**。

```css
ul.unorder_list{
  list-style: circle;
}
```

可再藉由 **margin** 和 **padding** 將預設的樣式消息。例：

```css
ul.unorder_list{
  list-style: circle;
  margin:0;
  padding:0;
}
```

## 範例



