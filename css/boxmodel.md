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

```
margin: 10px;                /* 上、右、下、左，皆 10px */
margin: 10px 20px;           /* 上、下皆 10px；左右皆 20px */
margin: 10px 20px 30px;      /* 上 10px；左右皆 20px；下 30px */
margin: 10px 20px 30px 40px; /* 按照上、右、下、左的順序，依序為 10px、20px、30px、40px */
```

## 區塊大小\(box-sizing\)

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

