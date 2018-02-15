# 3.10 表單樣式

## 文字欄位\(type="text"\)

`:focus`：某欄位取得滑鼠焦點時。也可應用在其它輸入框，例： `textarea` 等。

HTML

```html
<input type="text" class="the_text">
```

CSS

```css
input.the_text:focus{
  border:5px solid red;
}
```

結果呈現：

![](/assets/focus_status.png)

## 多文字欄位\(textarea\)

HTML

```html
<textarea rows="3" cols="50">這是內容</textarea>
```

CSS

```css
textarea{
  /* resize: both; */
}
```

結果如下：

![](/assets/textarea_resize_sample.png)resize 可選的值有：

* both：這是預設。使用者可改變 textarea 欄位的寬高。
* horizontal：使用者可水平將 textarea 欄位變寬。
* vertical：使用者可垂直將 textarea 欄位變高。
* none：使用者無法改變 textarea 欄位的寬高。

## 留意：預設難以客製化的項目

* 單選框\(type="radio"\)
* 核取框\(type="checkbox"\)
* 下拉選單\(select\)

![](/assets/form_difficult_customize.png)

