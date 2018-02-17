# 3.13 圓角

## 範例：基本語法

HTML

```html
<div class="test_radius">這是 div 的內容</div>
```

CSS

```css
div.test_radius{
  width: 100px;
  height: 100px;
  border:1px solid red;

  border-radius: 10px; /* 左上、右上、右下、左下，四個角，都會變成 10px 的圓角 */
}
```

如圖：

![](/assets/border_radius1.png)

繪製原理\(下圖是以其中一個角為例\)：

![](/assets/border_radius_theory.png)

## 各種寫法

圓角順序：左上、右上、右下、左下。

```
border-radius: 1px 2px 3px 4px;
```

圓角順序：

