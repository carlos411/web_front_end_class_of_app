# 4.1.11 變數可視範圍\(scope\)

一個變數的可視範圍，指的是哪些程式可以存取該變數。

所以當宣告了一個變數之後，要能夠區別該變數的 scope。

## 範例 1：先後順序

```js
alert(a); // 會跳出提示訊息，內容為 undefined。因為在這行之前，a 並沒有被宣告成變數過。
var a = 10;
```

## 範例 2

```js
var a = 10;
function add_number(){
  a = a + 10;
}
add_number();
alert(a); // 跳出提示訊息，結果 a 是 20。
```

## 範例 3

```js
var a = 10;
function add_number(a){
  a = a + 10;
  alert(a); // 跳出提示訊息，結果 a 是 20。
}
add_number(a);
alert(a); // 跳出提示訊息，結果 a 是 10。
```

## 範例 4

```js
var a = 10;
function add_number(x){
  a = x + 10;
}
add_number(a);
alert(a); // 跳出提示訊息，結果 a 是 20。
alert(x); // 跳出提示訊息，結果為 undefined。
```



