# 4.3.3 非同步的 JavaScript 與 XML 技術 AJAX - 使用 jQuery

jQuery 將原來需要寫很多行的 JavaScript，包裝成單一函式，便於使用。

```js
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>jQuery AJAX</title>
  </head>
  <body>
    <button type="button" id="the_button">取得資料</button>
    <div id="get_data"></div>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <script>
      $("#the_button").on("click", function(){
        $.ajax({
          url: 'http://notes.carlos-studio.com/ajax/example.php', // 將資料傳送出去的網址
          type: 'get', // 也可以是POST
          data: 'a=1', // 傳遞的參數
          dataType: 'json', // 傳回來的資料類型
          success: function(data){ // 成功後會執行的函式
            //console.log(data);
            $("#get_data").html(data.value);
          }
        });
      });
    </script>
  </body>
</html>
```

## 其它資源

[jQuery 的 Ajax 完整官網資源](http://api.jquery.com/jQuery.ajax/)

