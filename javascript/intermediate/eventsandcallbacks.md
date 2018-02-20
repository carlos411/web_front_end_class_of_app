# 4.2.2 事件\(event\)和回呼函式\(callback\)

回顧最一開始的範例：

```html
<h1>這是內文標題</h1>
```

```js
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

## 常用 window 事件

* onload
* onresize

## 常用的表單事件

* onfocus
* onsubmit

事件列表參考：[https://www.w3schools.com/tags/ref\_eventattributes.asp](https://www.w3schools.com/tags/ref_eventattributes.asp)

