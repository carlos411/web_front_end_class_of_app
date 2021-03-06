# 4.3.4 儲存機制 - 本地端儲存\(localstorage\)

localStorage 是在 HTML 5 時，才有的功能。相對於 cookie ，localStorage 有更多的儲存空間\(大約 5MB\)，且有較多的函式方便使用。

之前做的專案：[團購導購地圖](http://notes.carlos-studio.com/55555map/map.php)。

在 `2_practice` 資料夾下，建立一個 `localstorage.html` 檔來測試練習。內容如下：

```markup
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>localStorage</title>

  </head>
  <body>
    <p>測試</p>

    <script>
      // 撰寫 JS 相關
    </script>
  </body>
</html>

```

## 儲存

於 console 分頁當中，輸入以下\(有兩種語法\)：

```javascript
// 語法一
localStorage.setItem("key_name", "key_value");

// 語法二
localStorage["key_name"] = "key_value";
```

下圖可看到在 Application → Storage → Local Storage 中，已儲存了一個「鍵的名稱為 **key\_**_**name**，該鍵之值為 **key\_value**_」

![](../../.gitbook/assets/localstorage_1.png)

註：儲存進去的值，皆會是字串形態。如果執行 `localStorage.setItem("dollar", 1);`，會儲存成 "1" 字串。可取出後，再透過 `parseInt()` 函式，轉成整數形態即可。

儲存「物件\(Object\)」前，需要先變成字串\(透過 **`JSON.stringify()`** 函式\)，例：

```javascript
localStorage.setItem("car", JSON.stringify({doors: 4, brand_name: "toyota"}));
```

## 取得

```javascript
// 語法一
var get_value = localStorage.getItem("key_name"); // get_value 的值為 key_value

// 語法二
var get_value = localStorage["key_name"];  // get_value 的值為 key_value
```

取得物件字串時，需再透過 **`JSON.parse()`** 函式，轉成物件格式，例：

```javascript
var get_car = JSON.parse(localStorage["car"]);

// 於 console 中查看取得的資料
console.log(get_car);
console.log(get_car.doors);
```

## 刪除

移除特定 key 及所對應的值：

```javascript
localStorage.removeItem("key_name");
```

## 全部刪除

將 localStorage 中的全部資料都清除：

```javascript
localStorage.clear();
```

