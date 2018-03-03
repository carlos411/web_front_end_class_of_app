# 2.16 表單 - &lt;form&gt;...&lt;/form&gt;

提供許多欄位，讓使用者填入後，送出資料。

## 基本結構

```html
<form action="#" method="#">
  ...
</form>
```

**action**：值是一個網址，代表要將使用者填入的資料，送至此網址。

**method**：可以是 **get** 或 **post**。若是 get 的話，表示資料會呈現於網址當中，post 則不會出現在網址當中，相對較安全。

get 範例：[http://carlos-studio.com/?address=abc&zone-234](http://carlos-studio.com/**?address=abc&zone-234**`)，資料以 **?** 做開始，以 **&** 做分隔。address 是欄位名稱\(name\)，**=** 後面緊接著是address 的值

## 文字框

```html
<input type="text" name="address" value="這是內容" placeholder="提示文字">
```

## 多行文字框

```html
<textarea name="content" rows="3" cols="50" placeholder="提示文字">這裡是文字</textarea>
```

實務上 rows 和 cols 較少用，因為可透過 CSS 來改變。

## 單選

**name** 要一樣，才能被視為單選：

```html
<input type="radio" name="custom_name" value="1" checked> 是
<input type="radio" name="custom_name" value="2"> 否
```

`checked`：是表示要選取的意思。

## 勾選

```html
<input type="checkbox" name="habits" checked> 興趣1
```

`checked`：勾選。

## 下拉選單

```html
<select name="country">
  <option value="1" selected>選項1</option>
  <option value="2">選項2</option>
  <option value="3">選項3</option>
</select>
```

`selected`：表示預設為這項。

## 按鈕

```html
<button type="button">這是一般按鈕</button>
```

## 資料送出按鈕 - submit

```html
<button type="submit">這是資料送出按鈕</button>
<!-- 或 -->
<input type="submit" value="這是資料送出按鈕">
```

## 範例練習

```html
<form action="#" method="get">
  <input type="text" name="address">
  <br>
  <textarea name="content">這裡是文字</textarea>
  <br>
  <input type="radio" name="custom_name" value="1"> 是
  <br>
  <input type="radio" name="custom_name" value="2"> 否
  <br>
  <input type="checkbox" name="habits"> 興趣1
  <br>
  <select name="country">
    <option value="1">選項1</option>
    <option value="2">選項2</option>
    <option value="3">選項3</option>
  </select>
  <br>
  <button type="button">這是一般按鈕</button>
  <br>
  <button type="submit">這是資料送出按鈕</button>
  <!-- 或 -->
  <br>
  <input type="submit" value="這是資料送出按鈕">
</form>
```

結果呈現：

![](/assets/表單基礎.png)

