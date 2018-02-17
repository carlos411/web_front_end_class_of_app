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

## 繪製原理

以「左上角」為例：

![](/assets/border_radius_theory.png)

## 各種寫法範例

圓角順序：左上\(1px\)、右上\(2px\)、右下\(3px\)、左下\(4px\)：

```css
border-radius: 10px 20px 30px 40px;
```

圓角順序：左上\(1px\)、右上及左下\(2px\)、右下\(3px\)：

```css
border-radius: 10px 20px 40px;
```

![](/assets/border_radius_ex2.png)

圓角順序：左上及右下\(10px\)、右上及左下\(20px\)：

```css
border-radius: 10px 20px;
```

![](/assets/border_radius_ex1.png)

上述的單位，也都可以改用百分比。

