# 4.1.2 註解

JS 註解有二種：

* 單行註解：以 `//` 雙斜線開頭，該行後面的文字都會被視為註解。
* 多行註解：以 `/*` 開頭，以 `*/` 結束，在此 2 個符號之間的文字，都會被視為註解。

```js
<body>
  <p>開啟 alert 提示訊息</p>

  <script type="text/javascript">
    var p = document.getElementsByTagName("p")[0];
    p.addEventListener("click", function(){
      alert("open dialog");
    });
  </script>
</body>
```

**註解的用意**：給「人」看的，瀏覽器遇到註解符號，會直接跳過，並**不會顯示於網頁**上，但會顯示於「**頁面原始碼**」中。

