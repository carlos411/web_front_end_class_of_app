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

## 文字框

```html
<input type="text">
```

## 多行文字框

```html
<textarea>這裡是文字</textarea>
```

## 單選

```html
<input type="radio" name="custom_name" value="1"> 是
<input type="radio" name="custom_name" value="2"> 否
```

## 多選

```
<input type="checkbox">
```



