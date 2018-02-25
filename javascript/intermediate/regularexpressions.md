# 4.2.8 表單驗證\(validation\) - 正規表示式

## 正規表示式 - Regular Expression

定義一個字串的規則格式，例如行動電話號碼

```js
// 定義一個比對的規則：字串內，一定要有「the book」。
var pattern = /the\s{1}book/;

// 定義一個字串
var str = "the book";

alert(pattern.test(str));
```

## 表單驗證



