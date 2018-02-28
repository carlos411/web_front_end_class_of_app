# 4.3.3 非同步的 JavaScript 與 XML 技術 AJAX - 使用 jQuery

jQuery 將原來需要寫很多行的 JavaScript，包裝成單一函式，便於使用。

```js
$.ajax({
  url: 'a.html',            // 將資料傳送出去的網址
  type: 'get',              // 也可以是POST
  data: 'ab='+ab,           // 傳遞的參數
  dataType: 'json',         // 傳回來的資料類型
  success: function(data){  // 成功後會執行的函式
    console.log(data);
  }
});
```

## 其它資源

[jQuery 的 Ajax 完整官網資源](http://api.jquery.com/jQuery.ajax/)

