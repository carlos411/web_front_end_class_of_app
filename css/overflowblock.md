# 3.19 overflow

當內容超出元素區域的，用來定義該如何處理超出的內容。常見可選的值有：

* `visible`：這是預設值，即正常出現。
* `hidden`：直接隱藏。
* `scroll`：出現捲軸來滑動內容。

## 範例 1：垂直方向

html

```markup
<div class="test_div">這是 div 的內容這是 div 的內容這是 div 的內容這是 div 的內容這是 div 的內容</div>
```

css

```css
div.test_div{
  border:2px solid red;
  width: 100px;
  height: 100px;
}
```

結果如圖：

![](../.gitbook/assets/overflow_1.png)

css 改成：

```css
div.test_div{
  border:2px solid red;
  width: 100px;
  height: 100px;

  /* 加上以下這行 */
  overflow: hidden;
}
```

結果如圖：

![](../.gitbook/assets/overflow_2.png)

或 css 改成如下：

```css
div.test_div{
  border:2px solid red;
  width: 100px;
  height: 100px;

  /* 加上以下這行 */
  overflow: scroll;
}
```

![](../.gitbook/assets/overflow_3.png)

## 範例 2：水平方向

html

```markup
<div class="test_div">這是 div 的內容這是 div 的內容這是 div 的內容這是 div 的內容這是 div 的內容</div>
```

css

```css
div.test_div{
  border:2px solid red;
  width: 100px;

  white-space: nowrap; /* 遇到空白的話，限制該行不要斷行 */
}
```

結果如圖：

![](../.gitbook/assets/overflow_4.png)

將 css 改成：

```css
div.test_div{
  border:2px solid red;
  width: 100px;

  white-space: nowrap; /* 遇到空白的話，限制該行不要斷行 */

  /* 加上以下兩行 */
  overflow: scroll;
  height: 40px;
}
```

結果如圖：

![](../.gitbook/assets/overflow_5.png)

## 應用：限制單行，超出的話，尾端出現 `…` 省略符號

```css
div.test_div{
  border:2px solid red;
  width: 100px;

  white-space: nowrap;      /* 不斷行 */
  overflow: hidden;         /* 隱藏 */
  text-overflow: ellipsis;  /* 出現省略符號 */
}
```

結果如圖\(文字超出部份，直接出現省略符號\)：

![](../.gitbook/assets/overflow_6.png)

