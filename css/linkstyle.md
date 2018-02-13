# 3.7 連結樣式

「連結」是以 `<a href="#">這是連結的文字</a>` 這樣的形式出現於網頁之中，其中有幾種基本的型態：

* 未點擊過的連結\(`:link` 預設\)
* 已點擊過的連結\(`:visited`\)
* 滑鼠移過去之後，文字的顏色\(`:hover`\)
* 滑鼠按壓下去不放後，文字的顏色\(`:active`\)

## 擬似類別\(Pseudo-class\)

針對連結專有的擬似類別，即這四種：`:link`、`:visited`、`:hover`、`:active`。

## 範例

HTML：

```html
<a href="#" class="link_style">這是連結文字</a>
```

CSS：

```css
.link_style{

}
```



