# 2.13 嵌入內容 - &lt;iframe&gt;...&lt;/iframe&gt;

`<iframe>`：inline frame 的縮寫。

## 語意

嵌入其他內容在目前的網頁，可以是網頁、影片等形式，最常應用在 youtube 提供的影片嵌入。

## 結構

```html
<iframe src="#"></iframe>
```

## 常用屬性

```html
<iframe src="#" width="100%" height="200px" frameborder="0"></iframe>
```

**width**：指定寬度，可以是 **%**、**px**。

**height**：指定高度，可以是 **%** 、**px**。

**frameborder**：是否要顯示邊框，**0** 表示不顯示，**1** 則為顯示。

## 範例 1

嵌入外部網站的內容

```html
<iframe src="https://dictionary.cambridge.org/dictionary/english-chinese-traditional/table"></iframe>
```

![](/assets/iframe_嵌入外部網站.png)

## 範例 2

嵌入 youtube 影片

![](/assets/iframe 嵌入影片.png)

![](/assets/iframe 嵌入影片.png)

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/1UWI7epjcBk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
```

結果呈現

![](/assets/iframe 嵌入影片結果.png)

## 練習

在您的網頁上試試 &lt;iframe&gt; 的呈現結果。

