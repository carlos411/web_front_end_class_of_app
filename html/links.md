# 2.10 連結 - &lt;a&gt;...&lt;/a&gt;

`<a>`：anchor，表示錨點的意思。

## 範例 1

基本語法

```html
<a href="http://tw.yahoo.com">這是連結</a>

<!-- 習慣上，有的時候暫時還沒有連結的時候，習慣先以 # 代替 -->
<a href="#">這是連結</a>
```

## 範例 2

屬性 target 的常用值：

* \_self：這是預設值，原分頁開 href 所指定的連結。
* \_blank：開新分頁。

```html
<a href="http://tw.yahoo.com" target="_blank">這是連結</a>
```

## 其他說明

連結的文字**顏色**，對使用者來說，有分四種，分別是：

* 未點擊過的連結\(`:link` 預設\)
* 已點擊過的連結\(`:visited`\)
* 滑鼠移過去之後，文字的顏色\(`:hover`\)
* 滑鼠按壓下去不放後，文字的顏色\(`:active`\)

## 練習

1、請試試連結加上 target 屬性，看看差異。

2、小應用：target 如果隨意指定其他名稱？例如：mywindow

3、請貼上以下的 style，看看差異：

```css
<style>
  /* 未點擊過的連結 */
  a:link{
    color: #000000;
  }
  /* 已點擊過的連結 */
  a:visited{
    color: #FF0000;
  }
  /* 滑鼠移過去之後，文字的顏色 */
  a:hover{
    color: #00FF00;
  }
  /* 滑鼠按壓下去不放後，文字的顏色 */
  a:active{
    color: #0000FF;
  }
</style>
```



