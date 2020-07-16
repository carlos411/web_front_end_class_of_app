# 2.4 中介資料\(Meta Data\)

## 語意

該網頁的額外資料，例如關鍵字、簡易描述等資訊，會被瀏覽器解讀。

注意：**&lt;meta&gt;** 沒有結尾標籤。

## 範例 1

```markup
<head>
  <meta charset="utf-8">
</head>
```

瀏覽器會解讀：該網頁的字元集編碼為 **utf-8**。即支援大多數的文字種類。

## 範例 2

```markup
<head>
  <meta name="keywords" content="HTML, CSS, JavaScript">
  <meta name="description" content="網站前端教學">
  <meta http-equiv="refresh" content="3">
  <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=yes">
</head>
```

`keywords`: 代表此頁面的關鍵字，雖然權重沒那麼高了，但建議養成習慣，加上去比較好。

`description`：有可能會顯示在 google 搜尋結果的說明當中。

`refresh`：此頁面每隔幾秒會重新整理一次。

`viewport`：指的是可視範圍。桌機版的瀏覽器，viewport 的寬度就等於瀏覽器的寬度。所以 viewport 通常是針對手機版的網頁在使用，指定 viewport 的 width 為設備寬度\(device-width\)；初始放大倍率\(`initial-scale`\)為1；是否要讓使用者可以用手指去縮放內容\(user-scalable\)。

## 總結

`<head>...</head>` 區段，都至少要有以下資訊：

```markup
<head>
  <meta charset="utf-8">
  <title>商品名稱 | 商品類別 | 品牌名稱</title>
  <meta name="keywords" content="HTML, CSS, JavaScript, 關鍵詞組">
  <meta name="description" content="網頁簡短描述，儘量在 70 字以內。">
  <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=yes">
</head>
```

請將 `keywords`、`description`、`viewport` 這三個 meta data，加到自己的網頁當中。

## 資源

[更多 Meta Data：https://www.w3schools.com/tags/tag\_meta.asp](https://www.w3schools.com/tags/tag_meta.asp)

{% hint style="info" %}
練習：

試試看範例 2 的 **http-equiv="refresh"** 是否正常運作。
{% endhint %}

## 其它

[FB 分享的 meta tag: Open Graph tag](https://developers.facebook.com/docs/sharing/webmasters/#markup)

