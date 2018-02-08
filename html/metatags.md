# 2.4.1 中介資料\(Meta Data\) - &lt;meta&gt;

## 語意

該網頁的額外資料，會被瀏覽器解讀。

注意：**&lt;meta&gt;** 沒有結尾標籤。

## 範例

```html
<head>
  <meta charset="utf-8">
</head>
```

瀏覽器會解讀：該網頁的字元集編碼為** utf-8**。即支援大多數的文字種類。

## 其他 Meta 範例

```html
<head>
  <meta name="keywords" content="HTML, CSS, JavaScript">
  <meta name="description" content="網站前端教學">
  <meta http-equiv="refresh" content="3">
</head>
```

`keywords`: 代表此頁面的關鍵字，雖然權重沒那麼高了，但建議養成習慣，加上去比較好。

`description`：有可能會顯示在 google 搜尋結果的說明當中。

`refresh`：此頁面每隔幾秒會重新整理一次。

## 資源

[https://www.w3schools.com/tags/tag\_meta.asp](https://www.w3schools.com/tags/tag_meta.asp)

