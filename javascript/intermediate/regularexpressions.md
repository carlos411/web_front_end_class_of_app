# 4.2.8 表單驗證\(validation\) - 正規表示式

## 正規表示式 - Regular Expression

* 定義一個字串的規則格式：寫法為 `/正規表示式/`。

* 再使用 `.test()` 方法，來驗證給定的字串是否符合規則，是的話回傳 `true`，反之回傳 `false`。

例：

```js
// 定義一個比對的規則：字串內，一定要有「the book」。\s{1} 表示僅能有1個空格。
var pattern = /the\s{1}book/;

// 想要比對的字串
var str = "the book";

// 顯示提示訊息，訊息為 true
alert(pattern.test(str));
```

## 表單驗證



