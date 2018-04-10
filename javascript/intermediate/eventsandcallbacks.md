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

```js
var h1 = document.getElementsByTagName("h1")[0];
h1.addEventListener("dblclick", function(){
  alert("open dialog");
});
```

## 常用 window 事件

* DOMContentLoaded：DOM 載入完成之後會觸發。
* onload：頁面中的所有物件\(含圖檔等\)都載入完成之後觸發：
* onresize：改變瀏覽器寬高時觸發。

```js
window.addEventListener("DOMContentLoaded", function(){
  alert("DOM 載入完成之後觸發。");
});
```

```js
window.addEventListener("load", function(){
  alert("所有資源載入完成之後觸發。");
});
```

```js
window.addEventListener("resize", function(){
  console.log("resize")
});
```

## 常用的表單事件

* onfocus：欄位取得焦點之後觸發。
* onblur：欄位失去焦點之後，會觸發。
* onchange：欄位內容改變時，會觸發。
* onkeyup：鍵盤按下去時，會觸發。
* onkeydown：鍵盤按下去放開後，會觸發。
* onsubmit：表單資料送出時觸發。

```html
<form id="the_form" action="#" method="get">
  <input type="text" id="text_input" name="title">
  <button type="submit">送出</button>
</form>
```

```js
text_input.addEventListener("focus", function(e){
  console.log("focus event");
})
```

```js
text_input.addEventListener("blur", function(e){
  console.log("blur event");
})
```

```js
text_input.addEventListener("change", function(e){
  console.log("change event");
})
```

```js
text_input.addEventListener("keydown", function(e){
  console.log(e); // 觀察 e
  console.log("keydown event: " + e.which);
})
```

```js
text_input.addEventListener("keyup", function(e){
  console.log(e); // 觀察 e
  console.log("keyup event: " + e.target.value);
})
```

關於 e，指的就是 event，js 內建在事件觸發時，帶入此物件，裡面包含了很多可用資訊。最後看一下 form 的 `onsubmit` 事件：

```js
var the_form = document.getElementById("the_form");
the_form.addEventListener("submit", function(e){
  // e.preventDefault(); 停止預設行為，表示不會送出資料
})
```

觀察開發者工具的 Network 頁籤。來看 post 資料。

![](/assets/form_network1.png)

![](/assets/form_network2.png)

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

事件列表參考：[https://www.w3schools.com/tags/ref\_eventattributes.asp](https://www.w3schools.com/tags/ref_eventattributes.asp)

