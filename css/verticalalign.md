# 3.15 排版 - 關於 vertical-align 對齊

同一個層級的元素當中，垂直方向的對齊方式。主要有三個可設定的值：

* top：垂直方向的對齊位置，上方對齊。
* middle：垂直方向的對齊位置，中間對齊。
* bottom：垂直方向的對齊位置，下方對齊。

## 範例

檔案所在路徑：`css/3.15/index.html`。

```markup
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

結果如圖：\(發現「第二項」、「第三項」都到下方了，通常可透過修改 `vertical-align` 來改變對齊方式\)

![](../.gitbook/assets/chui-zhi-fang-xiang-dui-qi-default.png)

將上述的 CSS 部份改成：

```css
ul li{
  display: inline-block;
  border:1px solid red;

  /* 垂直方向的對齊方式：上方對齊 */
  vertical-align:top;
}
```

![](../.gitbook/assets/chui-zhi-dui-qi-fang-xiang-top.png)

若將 vertical-align 改成 **middle**，則：

![](../.gitbook/assets/chui-zhi-dui-qi-fang-xiang-middle.png)

