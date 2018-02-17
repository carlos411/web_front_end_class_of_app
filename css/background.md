# 3.12 背景

## 背景單色

```css
div{
  background-color: red;
}
```

## 背景圖片

假設目前檔案結構如下：

* project/
* project/images/christmas-dark.png  \(註：此圖寬高大小皆為 200px。\)
* project/index.html

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

![](/assets/bg_image.png)

二、設定圖片的重覆狀態，使用 **background-repeat**：

可選的值有：

* repeat：預設，指的是圖片向 x 軸、y 軸重覆出現。
* repeat-x：圖片向 x 軸重覆出現。
* repeat-y：圖片向 y 軸重覆出現。
* no-repeat：不重覆，只出現一次。



