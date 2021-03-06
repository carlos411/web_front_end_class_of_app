# 2.13 嵌入內容

`<iframe>`：inline frame 的縮寫。

## 語意

嵌入其他內容在目前的網頁，可以是網頁、影片等形式，最常應用在 youtube 提供的影片嵌入。

## 結構

```markup
<iframe src="#"></iframe>
```

## 常用屬性

```markup
<iframe src="#" width="100%" height="200px" frameborder="0"></iframe>
```

**width**：指定寬度，可以是 **%**、**px**。

**height**：指定高度，可以是 **%** 、**px**。

**frameborder**：是否要顯示邊框，**0** 表示不顯示，**1** 則為顯示。

## 範例 1

嵌入外部網站的內容

```markup
<iframe src="https://dictionary.cambridge.org/dictionary/english-chinese-traditional/table"></iframe>
```

![](../.gitbook/assets/iframe-qian-ru-wai-bu-wang-zhan.png)

## 範例 2

嵌入 youtube 影片

![](../.gitbook/assets/iframe-qian-ru-ying-pian.png)

```markup
<iframe width="560" height="315" src="https://www.youtube.com/embed/1UWI7epjcBk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
```

結果呈現

![](../.gitbook/assets/iframe-qian-ru-ying-pian-jie-guo.png)

## 練習

檔案所在路徑：`html/2.13/index.html`

請開啟練習的檔案，使用了 iframe 載入 youtube 的影片及其它網站。

