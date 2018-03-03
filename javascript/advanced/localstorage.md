# 4.3.5 儲存機制 - 本地端儲存\(localStorage\)

localStorage 是在 HTML 5 時，才有的功能。相對於 cookie ，localStorage 有更多的儲存空間\(大約 5MB\)，且有較多的函式方便使用。

隨意開啟一個網頁或瀏覽\( [http://carlos-studio.com](http://carlos-studio.com%29 %29。開啟開發者工具%28`cmd + option + i`\) \) 來測試：

## 儲存

於 console 分頁當中，輸入以下\(有兩種語法\)：

```js
// 語法一
localStorage.setItem("key_name", "key_value");

// 語法二
localStorage["key_name"] = "key_value";
```

下圖可看到在 Application → Storage → Local Storage 中，已儲存了一個「鍵的名稱為 **key\_**_**name**，該鍵之值為 **key\_value**_」

![](/assets/localstorage_1.png)

註：儲存進去的值，皆會是字串形態。如果執行 `localStorage.setItem("dollar", 1);`，會儲存成 "1" 字串。可取出後，再透過 `parseInt()` 函式，轉成整數形態即可。

## 取得

```js
// 語法一
var get_value = localStorage.getItem("key_name"); // get_value 的值為 key_value

// 語法二
var get_value = localStorage["key_name"];  // get_value 的值為 key_value
```

## 刪除

移除特定 key 及所對應的值：

```js
localStorage.removeItem("key_name");
```

## 全部刪除

將 localStorage 中的全部資料都清除：

```js
localStorage.clear();
```



