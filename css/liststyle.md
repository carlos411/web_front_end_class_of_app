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

## 範例：各種 list-style 所呈現的標號

HTML

```html
<ul class="unorder_list">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -circle">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -decimal">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -none">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -inside">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -lower-alpha">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -lower-roman">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -square">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -upper-alpha">
  <li>第一項</li>
  <li>第一項</li>
</ul>
<ul class="unorder_list -upper-roman">
  <li>第一項</li>
  <li>第一項</li>
</ul>
```

CSS

```css
ul.unorder_list{
}
ul.unorder_list.-circle{
  list-style: circle;
}
ul.unorder_list.-decimal{
  list-style: decimal;
}
ul.unorder_list.-none{
  list-style: none;
}
ul.unorder_list.-inside{
  list-style: inside;
}
ul.unorder_list.-lower-alpha{
  list-style: lower-alpha;
}
ul.unorder_list.-lower-roman{
  list-style: lower-roman;
}
ul.unorder_list.-square{
  list-style: square;
}
ul.unorder_list.-upper-alpha{
  list-style: upper-alpha;
}
ul.unorder_list.-upper-roman{
  list-style: upper-roman;
}
```

結果

![](/assets/list_basic2.png)

觀察 `list-style: inside;` 的樣子：![](/assets/list_inside.png)

