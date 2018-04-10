# 4.2.2 事件\(event\)和回呼函式\(callback\)

回顧最一開始的範例\(HTML 及 JS\)：

```js
<h1>這是內文標題</h1>
<script type="text/javascript">
  var h1 = document.getElementsByTagName("h1")[0];
  h1.addEventListener("click", function(){
    alert("open dialog");
  });
</script>
```

* **click**：就是一個事件，指的是滑鼠左鍵按一下，這樣的行為，就是一種事件\(event\)。

* **function\(\){...}**：這就是回呼函式\(callback\)，指的是完成一件事之後，所要執行的函式，就叫做 callback。

## 常用滑鼠事件

* onclick：滑鼠左鍵按一下。

* ondblclick：消鼠左鍵按兩下。

* onmousedown：滑鼠左鍵按下未抬起就會觸發。

* onmousemove：滑鼠游標在元素上移動。

* onmouseout：滑鼠移出元素。

* onmouseup：滑鼠左鍵按下後抬起時觸發。

註：大部份寫在 js 的事件時，前面的 `on` 都可省略。

## 常用 window 事件

* onload：頁面中的所有物件\(含圖檔等\)都完載入完成之後觸發：
* onresize：改變瀏覽器寬高時觸發。
* DOMContentLoaded：DOM 載入完成之後會觸發。

## 常用的表單事件

* onfocus：欄位取得焦點之後觸發。
* onsubmit：表單資料送出時觸發。

事件列表參考：[https://www.w3schools.com/tags/ref\_eventattributes.asp](https://www.w3schools.com/tags/ref_eventattributes.asp)

## 使用 HTML 事件屬性去觸發

不建議，通常事件會由 JS 去控制，HTML 儘可能保持乾淨、易讀。

例：\(留意 html 中的 **onclick 屬性** \)

```js
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>

  </head>
  <body>
    <h1 onclick="open_dialog()">這是內文標題</h1>

    <script type="text/javascript">
      function open_dialog(){
        alert("open dialog");
      }
    </script>
  </body>
</html>
```



