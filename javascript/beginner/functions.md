# 4.1.8 函式\(Function\)

什麼是函式？

多行的程式，組合在一起，變成一段 Code，可重覆在多處使用。

## 建立函式

![](/assets/function_basic1.png)

## 使用函式

範例：

```js
myFunction();

var result = myFunction();
```

## 傳遞參數及回傳結果

![](/assets/function_basic2.png)

## 練習

觀察程式的執行流程、函數的使用：

```js
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>

  </head>
  <body>

    <script type="text/javascript">
      var a = 1;
      var b = 2;
      function add(){
        a = a + 1; // a 結果變成 2
        b = b + 1; // b 結果變成 3
        alert(a+b); // 5
      }
      add(); // 執行 add() 函式

      var multiple = function(){
        a = a * 2; // a 結果變成 4
        b = b * 2; // b 結果變成 6
        alert(a*b); // 24
      };
      multiple(); // 執行 multiple() 函式

      var minus_one = function(x, y){
        x = x - 1; // x 結果 是 3
        y = y - 1; // y 結果 是 5
        return x - y; // 回傳 -2
      };
      var c = minus_one(a, b); // 執行 minus_one() 函式，並將回傳值賦予變數 c，所以 c 會是 -2
      alert(c);
    </script>

  </body>
</html>
```



