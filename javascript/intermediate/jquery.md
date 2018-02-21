# 4.2.3 jQuery 函式庫

一個 JavaScript 的函式庫，便於操控網頁元素，及提供各種方便的函式，讓開發者不用從頭開始做起。[官方網站](http://jquery.com/)。

## 如何在網頁中載入 jQuery 函式庫

### 方式一：下載後，於網頁中載入

第一步：到此網址： [http://jquery.com/download/](http://jquery.com/download/)

第二步：下載

![](/assets/jquery_download.png)

第三步：於網頁\(**index.html**\)中載入，假設資料夾的結構如下：

* js/jquery.js
* index.html



```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
    <style>
    h1{
      color: red;
    }
    </style>
  </head>
  <body>
    <h1>這是內文標題</h1>
    <script src="./js/jquery.js">

  </body>
</html>
```

## 使用範例

JavaScript 版本

```js
var h1 = document.getElementsByTagName("h1")[0];
```

jQuery 版本

```
var h1 = $("h1")
```



