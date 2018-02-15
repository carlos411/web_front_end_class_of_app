# 4.1.10 陣列\(Array\)

儲存多個值，在同一個變數裡。

![](/assets/array_syntax.png)

陣列裡的項目，起始項目是從 0 開始算起，以上圖範例來看，item1 是第 0  項、 item2 是第 1 項…以此類推。

## 建立陣列

語法

```js
// 宣告 cars 為一個陣列，儲存三個值
var cars = ["Saab", "Volvo", "BMW"];

// 也可以這樣寫(搭配斷行)，有時是易讀性
var cars = [
  "Saab",
  "Volvo",
  "BMW"
];

// 也可以這樣寫：
var cars = new Array("Saab", "Volvo", "BMW");

// 宣告 tables 為一個空的陣列，但沒有儲存任何東西
var tables = []
```

## 取得陣列裡的值

語法

```
var cars = ["Saab", "Volvo", "BMW"];

var car1 = cars[0];
```



