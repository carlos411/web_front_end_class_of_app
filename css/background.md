# 3.13 背景

## 背景單色

```css
div{
  background-color: red;
}
```

## 範例1：背景圖片

檔案所在路徑：`css/3.13/index.html`

假設目前檔案結構如下：

* project/
* project/images/christmas-dark.png  \(註：此圖寬高大小皆為 200px。\)
* project/index.html

christmas-dark.png 的圖片為：

![](../.gitbook/assets/christmas-dark.png)

在 index.html 檔案裡，指定如下 CSS：

一、顯示背景圖片，使用 **background-image**：

```css
<style>
body{
  background-image: url("./images/christmas-dark.png");
}
</style>
```

結果呈現：會發現此圖在 &lt;body&gt; 區域內，不斷地水平、垂直反覆出現圖片。

![](../.gitbook/assets/bg_image.png)

二、設定圖片的重覆狀態，使用 **background-repeat**：

```css
<style>
body{
  background-image: url("./images/christmas-dark.png");
  background-repeat: no-repeat; /* repeat-x repeat-y */
}
</style>
```

可選的值有：

* repeat：預設，指的是圖片向 x 軸、y 軸重覆出現。
* repeat-x：圖片向 x 軸重覆出現。
* repeat-y：圖片向 y 軸重覆出現。
* no-repeat：不重覆，只出現一次。

![](../.gitbook/assets/bei-jing-zhong-fu.png)

## 範例2：背景圖片

檔案所在路徑：`css/3.13/index_lion.html`

假設檔案結構如下：

* project/
* project/images/lion.png  \(註：此圖寬高大小為 640 x 428。\)
* project/index\_lion.html

lion.png 的圖片為：

![](../.gitbook/assets/lion.jpg)

index\_lion.html 檔案：

```markup
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>

    <style>
    div.place_img{
      width: 300px;
      height: 300px;
      border:1px solid red;

      background-image: url("./images/lion.jpg");
      background-repeat: no-repeat;
    }
    </style>

  </head>
  <body>
    <div class="place_img">這是 div 的內容</div>

  </body>
</html>
```

結果如下：背景圖超過 div 的區域，會被遮掉看不到。

![](../.gitbook/assets/background1.png)

### 使用 **background-size** 來設定背景圖的大小

```css
div.place_img{
  width: 300px;
  height: 300px;
  border:1px solid red;

  background-image: url("./images/lion.jpg");
  background-repeat: no-repeat;

  background-size: 80%; /* 背景圖的寬度會變成佔 div 區域的 80%。 */
  /*
  其它語法：
  background-size: 50% 50%; 背景圖的寬度及高度會變成佔 div 區域的 50%。圖片會變形。
  background-size: 150px 100px; 改成固定單位，寬為 150px，高為 100px。
  */
}
```

結果呈現：

![](../.gitbook/assets/background2.png)

特殊關鍵字\(**contain**\)：要讓圖片在區域內能夠完整呈現

```css
div.place_img{
  width: 300px;
  height: 300px;
  border:1px solid red;

  background-image: url("./images/lion.jpg");
  background-repeat: no-repeat;

  background-size: contain;
}
```

結果呈現：

![](../.gitbook/assets/background3.png)

如果將div的高度改成100px的話，則結果會變成：

![](../.gitbook/assets/background4.png)

特殊關鍵字\(**cover**\)：要讓圖片佔滿整個區域

```css
div.place_img{
  width: 300px;
  height: 300px;
  border:1px solid red;

  background-image: url("./images/lion.jpg");
  background-repeat: no-repeat;

  background-size: cover;
}
```

結果如圖：

![](../.gitbook/assets/background6.png)

### 使用 **background-position** 來設定背景圖的位置

```css
div.place_img{
  width: 300px;
  height: 300px;
  border:1px solid red;

  background-image: url("./images/lion.jpg");
  background-repeat: no-repeat;
  background-size: 80%;

  background-position: center bottom; /* 水平方向：置中；垂直方向：置底 */
}
```

結果如圖：

![](../.gitbook/assets/background7.png)

所以該圖在區域內，搭配關鍵字的話，共有以下幾種組合：

```css
background-position: left top;       /* 水平方向：置左；垂直方向：置頂 */
background-position: center top;     /* 水平方向：置中；垂直方向：置頂 */
background-position: right top;      /* 水平方向：置右；垂直方向：置頂 */
background-position: left center;    /* 水平方向：置左；垂直方向：置中 */
background-position: center center;  /* 水平方向：置中；垂直方向：置中 */
background-position: right center;   /* 水平方向：置右；垂直方向：置中 */
background-position: left bottom;    /* 水平方向：置左；垂直方向：置底 */
background-position: center bottom;  /* 水平方向：置中；垂直方向：置底 */
background-position: right bottom;   /* 水平方向：置右；垂直方向：置底 */
```

也可以指定水平方向、固定方向的距離，單位可以是 px 或 %：

```css
background-position: 50px 10px; /* 水平方向：離左側 50px 的距離；垂直方向：離上側 10px 的距離 */
```

結果如圖：

![](../.gitbook/assets/background8.png)

