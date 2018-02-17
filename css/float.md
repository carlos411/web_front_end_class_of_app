# 3.15 關於浮動\(float\)

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

結果：

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



