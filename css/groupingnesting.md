# 3.11 群組和巢狀寫法

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
<div>
  <p>段落一</p>
  <div>
    <p>段落二</p>
  </div>
</div>
```

## &gt;



