# 3.4 class 和 id

在 html 當中的任何標籤，都可以給定 **class** 和 **id** 這兩個屬性，例：

```html
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



