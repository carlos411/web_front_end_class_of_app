# 4.2.4 JS 與 jQuery 操控網頁元素 - 取得

HTML：

```html
<p>這是段落一</p>
<p id="the_id">這是段落二</p>
<p class="class_name">這是段落三</p>
<div class="class_name">這是 div 區塊</div>
```

JavaScript：

```js
document.getElementsByTagName("p");             // 取得 所有 <p> 元素
document.getElementById("the_id");              // 取得 id="the_id" 的元素
document.getElementsByClassName("class_name");  // 取得 class="class_name" 的元素
```

對應 jQuery：

```
$("p");
$("#the_id");
$(".class_name");
```



