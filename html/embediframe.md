# 2.13 嵌入內容 - &lt;iframe&gt;...&lt;/iframe&gt;

`<iframe>`：inline frame

## 語意

嵌入其他內容在目前的網頁，可以是網頁、影片等形式，最常應該在 youtube 提供的影片嵌入。

## 結構

```html
<iframe src="#"></iframe>
```

## 常用屬性

```
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

## 範例 2

嵌入 youtube 影片

