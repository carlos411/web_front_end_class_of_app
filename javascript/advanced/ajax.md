# 4.3.2 非同步技術 AJAX - 使用 JS

AJAX = **A**synchronous **J**avaScript **a**nd **X**ML。

## 同步資料請求

在程式的執行過程當中，一定要是一個接著一個，例如：第一行程式執行完後才會執行第2行。

例 1：for 迴圈跑完了5次之後，才會執行 `alert("done");`。絕對不可能先跑 `alert("done");`。

```js
for(var i = 0; i < 5; i++){
  alert(i);
}
alert("done");
```

第 2：下載的先後順序，且一定是 jQuery 程式執行完後，才會執行 bootstrap.js 程式。

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



