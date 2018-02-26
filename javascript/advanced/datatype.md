# 4.3.1 資料格式：XML 與 JSON

無論是同個系統或是多個系統之間，互相傳遞資料時，最常用的兩種格式，即 **XML** 與 **JSON**。都是純文字格式。

* XML = e**X**tensible **M**arkup **L**anguage。HTML 就是 XML 的其中一種。
* JSON = **J**ava**S**cript **O**bject **N**otation。

## 範例假設

有一個產品，品牌名稱為 `the_brand`，型號為 `t-123`，價格為 `100000`。圖片路徑有 [`http://ex.com/a.png`、`http://ex.com/b.png`](http://ex.com/a.png、http://ex.com/b.png) 。

請分別用 XML及 JSON 格式來表達：

## XML 格式

就像寫 HTML 一樣，只是現在可自行定義標籤名稱：

```xml
<?xml version="1.0" encoding="UTF-8"?>
<product>
  <brand>the_brand</brand>
  <model>t-123</model>
  <price>100000</price>
  <pictures>
    <source>http://ex.com/a.png</source>
    <source>http://ex.com/b.png</source>
  </pictures>
</product>
```

若想確認 XML 格式是否符合規範的話，可到 [XML Viewer](https://codebeautify.org/xmlviewer) 網站測試。如圖：

## JSON 格式

物件及陣列兩種格式都屬於 JSON 格式。

```json
{
  "brand": "the_brand",
  "model": "t-123",
  "price": "100000",
  "pictures":["http://ex.com/a.png", "http://ex.com/b.png"]
}
```

若想確認 JSON 格式是否符合規範的話，可到 [json parser](http://json.parser.online.fr/) 網站測試。如圖：

![](/assets/json_parser.png)

