# 4.1.3 變數\(variable\)和資料類型\(data type\)

## 用途

主要用途為**暫存資料**，將一個自行指定的「值\(Value\)」，存放在一個「變數名稱」當中。

可以想像成是一個有名稱的盒子\(變數\)，裡面裝著一個東西\(值\)，之後就可以重覆利用該盒子。

![](../../.gitbook/assets/bian-shu.png)

上圖的解讀：宣告了一個變數，它的名稱為 job，所存的值為 **web designer**。

其他注意事項：

* **=**：**等號** 將右邊的值，指定給左邊的變數名稱。
* **;**：**分號** 代表該行結束。
* ""：**雙引號**，代表一串文字，也可以改用單引號。
* 養成習慣，各個地方，都建議加上空格，以利閱讀性，例如等號的左右兩邊。
* 變數可以先宣告，在後面的程式碼當中，再賦予其值。

## 變數型態

先認識兩個變數型態

* 字串：以雙引號或單引號括起來，如上圖示意，我們就可以說「**job 這個變數的型態為字串**」。
* 數值：代表的是數學中的數值，可以是負數、零、正數、小數。例：「`var month = 2;`」。留意不需要有雙引號或單引號。

其它變數型態尚有：陣列、物件、null、undefined、浮點數、布林值。

## 範例

```javascript
var job = "web designer";
var month = 2;
var day;
var weight = 30.5;

day = 21;
```

