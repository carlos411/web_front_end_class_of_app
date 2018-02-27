# 4.3.2 非同步技術 AJAX - 使用 JS

AJAX = **A**synchronous **J**avaScript **a**nd **X**ML。

## 同步資料請求

在程式的執行過程當中，一定要是一個接著一個，例如：第一行程式執行完後才會執行第2行。

![](/assets/同步與ajax非同步_1.png)

例 1：for 迴圈跑完了5次之後，才會執行 `alert("done");`。絕對不可能先跑 `alert("done");`。

```js
for(var i = 0; i < 5; i++){
  alert(i);
}
alert("done");
```

第 2：下載的先後順序，jquery 會先請求下載，再來才是 bootstrap 程式。

且一定是 jQuery 程式執行完後，才會執行 bootstrap.js 程式。

```html
<!doctype html>
<html>
  <head>
    <script type="text/javascript" src="./js/jquery-1.11.1.min.js"></script>
    <script type="text/javascript" src="./js/bootstrap.js"></script>
  </head>
  <body>
  </body>
</html>
```

## 非同步資料請求

運作原理：

![](/assets/ajax_1.png)

B 段程式與 C 段程式，沒有先後的相依性，幾乎是同時執行\(或者B或C先執行\)。

因為 AJAX 非同步資料請求技術的問題，使用網頁局部刷新內容變得可以實現。

## JavaScript 實作 AJAX 的程式\(不建議使用\)

參考就好，因為現在已經有其它更方便的寫法。

HTML：

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Using XMLHttpRequest</title>
    <script type="text/javascript" src="./js/ajaxtest.js"></script>
  </head>
  <body>
    <a href="./data/message.txt" onclick="grabFile(this.href); return false;">點擊這裡取得 message.txt 檔案的內容</a>
  </body>
</html>
```

如圖：



