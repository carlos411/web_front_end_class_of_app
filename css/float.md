# 3.15 排版 - 關於浮動\(float\)

決定一個元素，在某區域的浮動狀態，可設定的值有：

* none：這是預設值
* left
* right

## 範例

HTML：

```html
<div class="first">
  <img src="./images/apple.png">
  這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容
</div>
```

CSS：

```css
div.first{
  width: 500px;
  border:1px solid red;
}
```

結果\(這是預設情況\)：

![](/assets/float1.png)

CSS 變更成：

```css
div.first{
  width: 500px;
  border:1px solid red;
}

/* 新增以下 */
div.first img{
  float:left;
}
```

結果：

![](/assets/float2.png)

CSS 再變更成：

```css
div.first{
  width: 500px;
  border:1px solid red;
}

/* 新增以下 */
div.first img{
  float: right;
}
```

結果：![](/assets/float3.png)

## 練習：問題

檔案所在路徑：`css/3.16/index.html`

當浮動區域的高度超出上層的高度時，上層的高度並不會增加，例：

HTML：

```html
<div class="first">
  <img src="./images/apple.png">
  這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是內容這是
</div>
```

CSS：

```css
div.first{
  width: 500px;
  border:1px solid red;
}
div.first img{
  float:right;
}
```

結果：發現紅框的高度，並沒有跟著圖片來增加，因為該圖已設定成浮動元素

![](/assets/flaot4.png)

## 解法：使用擬似元素\(Pseudo Element\) `::after`

修改 CSS 成：

```css
div.first{
  width: 500px;
  border:1px solid red;
}
/* 增加 ::after 這個擬似元素 */
/*
 1、在 div.first 的最尾端增加一個擬似元素，可放入內容
 2、內容這裡設定成內容為「abc」的內容
 3、將該元素設定成區塊元素
 4、使用 clear: both 來設定此元素的左右側，都不能有任何元素。
*/
div.first::after{
  content:"abc";
  display: block;
  clear:both;
}

div.first img{
  float:right;
}
```

結果：

![](/assets/float6.png)

故將 `content: "abc";` 改成 `content: "";`，即變成：![](/assets/float5.png)

