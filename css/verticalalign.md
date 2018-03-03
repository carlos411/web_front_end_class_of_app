# 3.15 關於 vertical-align 對齊

同一個層級的元素當中，垂直方向的對齊方式。主要有三個可設定的值：

* top：垂直方向的對齊位置，上方。
* middle：垂直方向的對齊位置，中間。
* bottom：垂直方向的對齊位置，下方。

## 範例

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
    <style>
    ul li{
      display: inline-block;
      border:1px solid red;
    }
    </style>
  </head>
  <body>
    <ul>
      <li>第一項<br>另一行</li>
      <li>第二項</li>
      <li>第三項</li>
    </ul>
  </body>
</html>
```

結果如圖：

![](/assets/垂直方向對齊_default.png)

將上述的 CSS 部份改成：

```css
ul li{
  display: inline-block;
  border:1px solid red;
  vertical-align:text-top;
}
```


