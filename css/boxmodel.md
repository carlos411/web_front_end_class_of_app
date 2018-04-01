# 3.6 區塊模型\(Box Model\)

**margin**：border 往外的距離。

**padding**：內容與 border 的距離。

**border**：該元素的邊框。

![](/assets/box_model.png)

## 範例

第一步：增加 **border**。

HTML：

```html
<span class="span1">這是文字1</span>
```

CSS：

```css
.span1{
  /* 1px 的框線、實線、紅色 */
  border:1px solid red;
}
```

![](/assets/box_model_example.png)

第二步：增加 **padding**。

更改 CSS 如下：

```css
.span1{
  /* 1px 的框線、實線、紅色 */
  border:1px solid red;

  /* 內容與框線的上、右、下、左，距離都是 10px */
  padding: 10px;
}
```

![](/assets/box_model_example2.png)

第三步：增加 **margin**。

更改 css 如下：

```css
.span1{
  /* 1px 的框線、實線、紅色 */
  border:1px solid red;

  /* 內容與框線的上、右、下、左，距離都是 10px */
  padding: 10px;

  /* 框線與上、右、下、左，距離都是 20px */
  margin: 20px;
}
```

![](/assets/box_model_example3.png)

留意：上下 margin 與其他 margin 或 padding 相鄰時，有時會被自動合併，取最大值。

## margin 和 padding 縮寫簡介

分別都有:

* `margin-top`、`margin-right`、`margin-bottom`、`margin-left`
* `padding-top`、`padding-right`、`padding-bottom`、`padding-left`

```css
margin: 10px;                /* 上、右、下、左，皆 10px */
margin: 10px 20px;           /* 上、下皆 10px；左右皆 20px */
margin: 10px 20px 30px;      /* 上 10px；左右皆 20px；下 30px */
margin: 10px 20px 30px 40px; /* 按照上、右、下、左的順序，依序為 10px、20px、30px、40px */
```

padding 縮寫形式相同。

## 區塊大小\(box-sizing\)

常用的有兩個值：**content-box** 和 **border-box**：定義的是寬度從何處算起。

* `content-box`：設定 width 時，寬度指的是內容寬。\(這是預設值\)
* `border-box`：設定 width 時，寬度指的是從邊框也算進去。

html：

```html
<div class="test_div">這是 div 的內容</div>
```

css：

```css
div.test_div{
  border:2px solid red;
  width: 100px;
}
```

結果如圖：\(可以得知實際寬度會是 104px。如果有 padding-left、padding-right的話，也會再加上padding 的寬度。\)

![](/assets/box_sizing_1.png)

css 改成如下：

```css
div.test_div{
  border:2px solid red;
  width: 100px;
  
  /* 加上以下這行 */
  box-sizing: border-box;
}
```

結果如圖：\(可以發現寬度變成了 100px，也就是 border 及 padding 的寬度也會被包含在 width 所設定的寬度內。\)

![](/assets/box_sizing_2.png)

## 練習：學會觀察

檔案所在路徑：`css/3.6/index.html`

請使用以下的程式在瀏覽器中執行，並學會使用 console 來查看 box model 的各數值。

並試著改變 display 屬性的值來觀察，可選的有 `inline`、`inline-block`、`block`：

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
    <style>
    /* 以逗號區隔，各個樣式都是相同的，只是不同名稱 */
    .span1, .span2, .para1, .para2{
      border: 1px solid red;
      padding: 10px;
      margin: 20px;
    }
    .span1{
      /* display: */
    }
    .span2{
      /* display: */
    }
    .para1{
      /* display: */
    }
    .para2{
      /* display: */
    }
    </style>
  </head>
  <body>
    <span class="span1">這是文字1</span>
    <span class="span2">這是文字2</span>

    <p class="para1">這是段落1</p>
    <p class="para2">這是段落2</p>
  </body>
</html>
```

結果呈現：

試試看瀏覽器開發者工具中的 **Elements**。

以 Mac 電腦為例，使用 **Chrome 瀏覽器**，快速鍵 `cmd + option + i`，即可看到 **elements** 的頁籤。如圖：

![](/assets/box_model_example4.png)

