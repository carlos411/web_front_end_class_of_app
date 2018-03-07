# 3.7 連結樣式

「連結」是以 `<a href="#">這是連結的文字</a>` 這樣的形式出現於網頁之中，其中有幾種基本的型態：

* 未點擊過的連結\(`:link` 預設\)
* 已點擊過的連結\(`:visited`\)
* 滑鼠移過去之後，文字的顏色\(`:hover`\)
* 滑鼠按壓下去不放後，文字的顏色\(`:active`\)

## 擬似類別\(Pseudo-class\)

針對**連結**專有的擬似類別，即這四種：`:link`、`:visited`、`:hover`、`:active`。

主要是瀏覽器已判斷到該連結的不同狀態時，可提供額外的設定。

## 練習

檔案所在路徑：`css/3.7/index.html`

HTML：

```html
<a href="#" class="link_style">這是連結文字</a>
```

CSS：

```css
/* 未點擊過的連結：黑色 */
a.link_style{
  color: #000000;
}
/* 已點擊過的連結：紅色 */
a.link_style:visited{
  color: #FF0000;
}
/* 滑鼠移過去之後，文字的顏色：綠色 */
a.link_style:hover{
  color: #00FF00;
}
/* 滑鼠按壓下去不放後，文字的顏色：藍色 */
a.link_style:active{
  color: #0000FF;
}
```



