# 3.11 表單樣式

## 文字欄位\(type="text"\)

`:focus`：擬似類別，某欄位取得滑鼠焦點時。也可應用在其它輸入框，例： `textarea` 等。

HTML

```markup
<input type="text" class="the_text">
```

CSS

```css
input.the_text:focus{
  border:5px solid red;
}
```

結果呈現：

![](../.gitbook/assets/focus_status.png)

## 多文字欄位\(textarea\)

HTML

```markup
<textarea rows="3" cols="50">這是內容</textarea>
```

CSS

```css
textarea{
  /* resize: both; */
}
```

結果如下：

![](../.gitbook/assets/textarea_resize_sample.png)

resize 可選的值有：

* both：這是預設。使用者可改變 textarea 欄位的寬高。
* horizontal：使用者可水平將 textarea 欄位變寬。
* vertical：使用者可垂直將 textarea 欄位變高。
* none：使用者無法改變 textarea 欄位的寬高。

## 留意：預設難以客製化的項目

* 單選框\(type="radio"\)：radio 邊框、背景等皆無法改變。
* 核取框\(type="checkbox"\)：checkbox 邊框、背景等皆無法改變。
* 下拉選單\(select\)：僅能部份改變。\(option 項目無法改變。\)

![](../.gitbook/assets/form_difficult_customize.png)

![](../.gitbook/assets/form_difficult_customize2.png)

這些項目若要有比較特別的介面，都需要高度客製化，都需再撰寫 html、css 、js 來做介面。

範例\(同學先參考即可\)：

{% embed url="https://codepen.io/carlos411/pen/WxojBK" caption="雙態開關按鈕" %}



