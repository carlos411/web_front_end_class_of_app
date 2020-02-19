# 3.4 class 和 id

在 html 當中的任何標籤，都可以給定 **class** 和 **id** 這兩個屬性：

**class**：表示樣式表的名稱。該名稱可以套用至多個元素上。

**id**：表示該元素的唯一名稱。在一個網頁當中，同樣的 id 名稱，不能重覆。

## 範例 1

```markup
<h1 class="title1">這是內文標題</h1>
<p id="the_para">這是段落</p>
```

這時，在 css 中，就可以透過 class 或 id 來套上樣式。例：

```css
/* . 符號表示 class 的名稱 */
.title1{
  color: blue;
}

/* # 符號表示 id 的名稱 */
#the_para{
  color: red;
}
```

## 範例 2

同一個元素，可以套用多個樣式名稱，以 **空格** 來做區隔，如下範例，會套用 **title1** 和 **change\_size** 這兩個樣式：

```markup
<h1 class="title1 change_size">這是內文標題</h1>
```

這時 `<h1>` 會套用以下兩個 CSS 的樣式表：

```css
.title1{
  color: blue;
}

.change_size{
  /* 文字大小設定成 20px */
  font-size: 20px;
}

.title1.change_size{
  text-decoration: underline;
}
```

註：**id** 屬性就沒有這種特性，一個元素不能有不同的 id。

