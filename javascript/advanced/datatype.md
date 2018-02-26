# 4.3.1 資料格式：XML 與 JSON

無論是同個系統或是多個系統之間，互相傳遞資料時，最常用的兩種格式，即 **XML** 與 **JSON**。都是純文字格式。

* XML = e**X**tensible **M**arkup **L**anguage。HTML 就是 XML 的其中一種。
* JSON = **J**ava**S**cript **O**bject **N**otation。

## 範例假設

有一個產品，品牌名稱為 `the_brand`，型號為 `t-123`，價格為 `100000`。圖片路徑有 [`http://ex.com/a.png`、`http://ex.com/b.png`](http://ex.com/a.png、http://ex.com/b.png) 。

請分別用 XML及 JSON 格式來表達：

## XML 格式

```
<item>
  <brand>the_brand</brand>
  <model>t-123</model>
</item>
```

## JSON 格式



