# 4.3.4 儲存機制 - cookie

![](/assets/cookie.png)

## 什麼是 Cookie？

Cookie 是網站在您瀏覽網頁時儲存在您的電腦上的資料。

Cookie 可用於儲存各種資訊，包含個人識別資訊（例如姓名、電子信箱、家中與公司電話住址……等等）。不過網站所能儲存使用的資料，也只有您確實輸入過的內容。網站無法自行取得您沒有提供過的資料，也不能任意存取您電腦內的檔案。

## 在哪裡可看到 cookie 資訊？

以 Chrome 瀏覽器為例：如下圖\(`cmd + option + i`，切換到 Application 頁籤\)

![](/assets/cookie_info1.png)

## 使用 JS 建立 cooke

```js
document.cookie = "school=某某大學";
```

通常沒有設定過期的時間的話，整個結束瀏覽器的話，該 cookie 就會自動被刪除。

![](/assets/cookie_info2.png)

## 設定 cookie 的過期時間

```js
document.cookie = "school=某某大學; expires=Thu, 18 Dec 2018 03:00:00 UTC";
```

![](/assets/cookie_info3.png)

註：[時間格式轉換](http://coderstoolbox.net/unixtimestamp/)

![](/assets/cookie_info4.png)

1970年1月1日0時0分0秒起至現在的總秒數

## 更改 cookie 的值

與建立 cookie 的語法是一樣的，只要 cookie 的名稱相同，就會直接更改相同名稱的 cookie。

## 刪除 cookie

## 取得 cookie 的值

## 



