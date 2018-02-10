# 2.14 span 和 div

`<span>...</span>`：\(不可考\)

`<div>...</div>`：document **div**isions。

## 語意

完全沒有語意的兩個標籤，就是 **span** 和 **div**。span 常用在一般文字要做不同的樣式或效果時會用到；div 常用在群組多個元素。

## 範例 1

span 常用於一般文字的部份。

```html
<p>這是一般文字，加<span>粗體</span>可能較好。</p>
```

## 範例 2

常用於將多個元素群組化成同一個。

```html
<div>
  <p>這是段落一</p>
  <p>這是段落二</p>
</div>
```

## 範例 3：理解 行內\(inline\) 與 區塊\(block\) 元素

```html
<div>
  <a href="#">這是連結一</a>
  <a href="#">這是連結二</a>
</div>

<div>
  <span>這是 span 1</span>
  <span>這是 span 2</span>
</div>

<div>
  <p>這是段落一</p>
  <p>這是段落二</p>
</div>
```

簡易判斷方法：若該元素會自動斷行，即為區塊\(block\)元素。

## 練習

理解 inline 元素 與 block 元素。

