# 4.1.6 條件式\(condition\)

運用 **true** 及 **false** 創造條件式。某條件為真，即執行一段程式，反之，則執行另一段程式。

## if 語法結構

![](/assets/condition_if.png)

## if else 語法結構

![](/assets/condition_if_else.png)

## if ... else if ... else 語法結構

`else if` 可以有多個。

![](/assets/condition_if_else_if_else.png)

## boolean 反轉符號：!

* 結果為 `true` 的話，前面加上 `!`，那結果就會變成 `false`。
* 結果為 `false` 的話，前面加上 `!`，那結果就會變成 `true`。

## switch 語法結構

結構一：

![](/assets/condition_switch.png)

結構二：

![](/assets/condition_switch_2.png)

## 練習

檔案所在路徑：`js/4.1.6/index.html`

請自行創立一個 html 檔案，貼上以下全部程式，用瀏覽器執行，觀察執行情況：

```js
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
  </head>
  <body>
    <script type="text/javascript">
      var a = 5;
      var b = 2;
      var c = "a";

      if(5 > 2){ // 試試 !，即這行變成 if(!(5 > 2)){
        alert("5 有大於 2。");
      }else{
        alert("5 沒有大於 2 是錯的。")
      }

      // 試試 拿掉 break、default、改變 c 的值為 "d"，看看各種執行情況
      switch(c){
        case "a":
          alert("是 a");
          break;
        case "b":
          alert("是 b");
          break;
        default:
          alert("這裡是 default");
      }
    </script>
  </body>
</html>
```



