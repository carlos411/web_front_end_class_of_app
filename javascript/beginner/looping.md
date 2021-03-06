# 4.1.7 迴圈\(loop\)

## for 迴圈

![](../../.gitbook/assets/loop_for.png)

範例：

```javascript
var x;
for(x = 0; x < 5; x++){
  alert(x);
}
// 繼續其他程式...
```

範例解讀：

第 1 步：宣告了一個變數，名稱為 x。

第 2 步：再來進行 for 迴圈，將 x 變數初始化為 0。

第 3 步：比較 x 是否小於 5，如果會的話，將持續進行以下步驟；如果不會的話，就 for 迴圈結束。

第 4 步：跳出 alert 訊息，訊息的內容就是 x 的值。

第 5 步：跑完大括號裡的程式碼，進行 `x++`，`x++` 的意思，等同於 `x = x + 1`，故 x 的結果變成是 1，然後回到第3步繼續判斷。

**注意：避免創造無窮迴圈。\(例如將** `x++` **改成** `x--`**\)。**

## while 迴圈

![](../../.gitbook/assets/loop_while.png)

範例：

```javascript
var i = 0;
while (i < 5) {
    alert(i);
    i++;
}
// 繼續其他程式...
```

範例解讀：

第 1 步：宣告了一個變數 i，其值為 0。

第 2 步：進行 while 迴圈，判斷 i 是否有小於 5。若有的話，執行大括號裡的程式；若沒有的話，跳離 while 迴圈。

第 3 步：跳出 alert 提示訊息，訊息即為 i 的值。再進行 `i++`，即等於 `i = i + 1`。回到步驟 2 繼續判斷。

**注意：避免創造無窮迴圈。\(例如：少寫了 i++ 這行\)。**

想想看，如果 i 的初始值是 6 的執行情況？

## do while 迴圈

![](../../.gitbook/assets/loop_do_while.png)

範例：

```javascript
var i = 0;
do{
  alert(i);
  i++;
} while (i < 5);
// 繼續其他程式...
```

範例解讀：

第 1 步：宣告了一個變數 i，其值為 0。

第 2 步：執行 do 區塊裡的程式，顯示 alert 提示訊息，再執行 `i++`，即 `i = i + 1`。

第 3 步：再判斷 i 是否有小於 5。若有的話，執行大括號裡的程式；若沒有的話，跳離 do while 迴圈。

**注意：避免創造無窮迴圈。\(例如：少寫了 i++ 這行\)。**

**do 區塊在一開始一定會執行 1 次，這是與 while 迴圈的主要差異之處。**

想想看，如果 i 的初始值是 6 的執行情況？

