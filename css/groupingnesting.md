# 3.11 群組和巢狀及其它符號寫法

## 逗號\(,\)

```css
div, p{
  color: red;
}
```

**&lt;div&gt;** 及 **&lt;p&gt;** 都會套用相同樣式。

## 空格

```css
div p{
  color: red;
}
```

**&lt;div&gt;** 內層的所有 **&lt;p&gt;** 才會套用到樣式。

例：\(**段落一**和**段落二**都會變成紅色。\)

```html
<p>段落一</p>
<div>
  <p>段落二</p>
  <section>
    <p>段落三</p>
  </section>
</div>
<p>段落四</p>
<p>段落五</p>
```

## 大於符號\(&gt;\)：第一層子元素

```css
div > p{
  color: red;
}
```

**&lt;div&gt;** 內層的第一層子元素 **&lt;p&gt;** 才會套用到樣式。

例：\(只有**段落一**會變成紅色。\)

```html
<p>段落一</p>
<div>
  <p>段落二</p>
  <section>
    <p>段落三</p>
  </section>
</div>
<p>段落四</p>
<p>段落五</p>
```

## 加號\(+\)：下個相鄰元素



