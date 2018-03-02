# 4.3.5 儲存機制 - 本地端儲存\(localStorage\)

相對於 cookie ，localStorage 有更多的儲存空間\(大約 5MB\)，且有較多的函式可以使用。

隨意開啟一個網頁或瀏覽\( [http://carlos-studio.com\](http://carlos-studio.com%29 %29。開啟開發者工具%28`cmd + option + i`\)來測試：

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

