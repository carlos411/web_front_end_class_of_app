# 4.2.5 JS 與 jQuery 操控網頁元素 - 更新

HTML：

```markup
<p id="the_id">這是段落</p>
```

CSS：

```css
.change_style{
  color: blue;
  font-size: 30px;
}
```

JavaScript：

* **innerHTML**：取得元素的內容。透過「=」，將元素的內容，整個取代。
* **setAttribute\(attribute, value\)**：更新屬性的值。
* **removeAttribute\(attribute\)**：移除屬性。

```javascript
// 透過 id 取得元素
var para_ele = document.getElementById("the_id");

// 提示訊息出現，得到元素的內容：「這是段落」
alert(para_ele.innerHTML);

// 改變該元素的內容
para_ele.innerHTML = "這是改變的文字";

// 元變元素的某個屬性  
// para_ele.setAttribute("style", "color: red;font-size: 30px;");  
para_ele.setAttribute("class", "change_style");

// 移除元素的屬性  
para_ele.removeAttribute("class");
```

針對 css 類別的新增及移除：

* **classList.add\("css 類別名稱"\)**：新增某類別。
* **classList.remove\("css 類別名稱"\)**：移除某類別。
* **classList.contains\("css 類別名稱"\)**：回傳 true or false，判斷是否有某個 css 類別。

## 對應的 jQuery 版本：

* **.html\(\)**：取得元素的內容。透過參數代入，將元素的內容，整個取代。
* **.attr\(attribute, value\)**：更新屬性的值。
* **.removeAttr\(attribute\)**：移除屬性。

```javascript
// 透過 id 取得元素
var para_ele = $("#the_id");

// 提示訊息出現，得到元素的內容：「這是段落」
alert($(para_ele).html());

// 改變該元素的內容
$(para_ele).html("這是改變的文字");

// 元變元素的某個屬性
// $(para_ele).attr("style", "color: red;font-size: 30px;");
$(para_ele).attr("class", "change_style");

// 移除元素的屬性
$(para_ele).removeAttr("class");
```

針對 css 類別的新增及移除：

* **addClass\("css 類別名稱"\)**：新增某類別。
* **removeClass\("css 類別名稱"\)**：移除某類別。
* **hasClass\("css 類別名稱"\)**：回傳 true or false，判斷是否有某個 css 類別。

## 練習

一、開啟以下兩個檔案觀察：

檔案所在路徑：`js/4.2.5/index.html`、`js/4.2.5/index_jquery.html`。

二、練習 css 類別的新增及移除：

html：

```markup
<p class="default_style" id="new_para">這是新增的段落</p>
<button type="button" id="btn_switch_style">新增/移除 another_style 樣式</button>
```

css：

```css
.default_style{
  color: red;
}

.another_style{
  font-size: 30px;
}
```

js：

```javascript
// 樣式的新增/移除：
var el_btn_switch_style = document.getElementById("btn_switch_style");
el_btn_switch_style.addEventListener("click", function(){
  var el_new_para = document.getElementById("new_para");
  if( el_new_para.classList.contains("another_style") ){
    el_new_para.classList.remove("another_style");
  }else{
    el_new_para.classList.add("another_style");
  }
});


// jQuery 版本：
$("#btn_switch_style").on("click", function(){

  if( $("#new_para").hasClass("another_style") ){
    $("#new_para").removeClass("another_style");
  }else{
    $("#new_para").addClass("another_style");
  }

});
```

