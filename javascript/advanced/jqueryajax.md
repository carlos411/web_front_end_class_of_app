# 4.3.3 非同步的 JavaScript 與 XML 技術 AJAX - 使用 jQuery

jQuery 將原來需要寫很多行的 JavaScript，包裝成單一函式，便於使用。

```js
$.ajax({
  url: 'http://notes.carlos-studio.com/ajax/example.php', // 將資料傳送出去的網址
  type: 'get',                                            // 也可以是 post
  data: 'a=1',                                            // 傳遞的參數
  dataType: 'json',                                       // 傳回來的資料類型
  success: function(data){                                // 成功接收到資料後，會執行的函式
    //console.log(data);
    $("#get_data").html(data.value);
  },
  statusCode: {                                           // 依據伺服器端回傳的狀態碼，來顯示錯誤訊息
    500: function() {
      alert( "500 伺服器端錯誤" );
    }
  }
});
```

## 完整範例

php

```php
<?php
header('Access-Control-Allow-Origin: *');
$arr = array('value' => "這個是回傳的資料");

echo json_encode($arr); // 產生：{"value":"這個是回傳的資料"}
?>
```

HTML 和 JavaScript

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
          type: 'get',                                            // 也可以是 post
          data: 'a=1',                                            // 傳遞的參數
          dataType: 'json',                                       // 傳回來的資料類型
          success: function(data){                                // 成功接收到資料後，會執行的函式
            //console.log(data);
            $("#get_data").html(data.value);
          },
          statusCode: {                                           // 依據伺服器端回傳的狀態碼，來顯示錯誤訊息
            500: function() {
              alert( "500 伺服器端錯誤" );
            }
          }
        });
      });
    </script>
  </body>
</html>
```

執行原理

![](/assets/jquery與ajax.png)

結果呈現

![](/assets/jquery與ajax_2.png)

## 其它資源

[jQuery 的 Ajax 完整官網資源](http://api.jquery.com/jQuery.ajax/)

