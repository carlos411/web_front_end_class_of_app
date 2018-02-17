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

一、顯示背景圖片：

```css
<style>
body{
  background-image: url("./images/christmas-dark.png");
}
</style>
```

結果呈現：

![](/assets/bg_image.png)

