# 4.1.11 變數可視範圍\(scope\)

一個變數的可視範圍，指的是哪些程式可以存取該變數。

所以當宣告了一個變數之後，要能夠區別該變數的 scope。

## 範例 1：先後順序

```js
alert(a); // 會跳出提示訊息，內容為 undefined。因為在這行之前，a 並沒有被宣告成變數過。
var a = 10;
```

## 範例 2

a 為全域變數

```js
var a = 10;
function add_number(){
  a = a + 10;
}
add_number();
alert(a); // 跳出提示訊息，結果 a 是 20。
```

## 範例 3

函式裡的 a 及 x ，在函式外就不存在。

```js
var a = 10;
function add_number(x){
  var a = x + 10;
  alert(a); // 跳出提示訊息，結果 a 是 20。
}
add_number(a);
alert(a); // 跳出提示訊息，結果 a 是 10。
```

## 範例 4

```js
var a = 10;
function add_number(a){
  a = a + 10;
  alert(a); // 跳出提示訊息，結果 a 是 20。
}
add_number(a);
alert(a); // 跳出提示訊息，結果 a 是 10。
```

## 範例 5：傳址呼叫\(call by reference\)

```js
var a = [1, 2];
function add_number(a){
  a.push(3);
}
add_number(a);
console.log(a); // 結果為 [1, 2, 3]
```

## 範例 5

```js
var a = 10;
function add_number(x){
  a = x + 10;
}
add_number(a);
alert(a); // 跳出提示訊息，結果 a 是 20。
alert(x); // 在 console 中，會出現 x is not defined 的錯誤訊息。
```

![](/assets/x_not_defined.png)

## 範例 6



