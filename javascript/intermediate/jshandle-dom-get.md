# 4.2.4 JS 與 jQuery 操控網頁元素 - 取得

## 元素

HTML：

```markup
<p>這是段落一</p>
<p id="the_id">這是段落二</p>
<p class="class_name">這是段落三</p>
<div class="class_name">這是 div 區塊</div>
```

JavaScript：

```javascript
document.getElementsByTagName("p");             // 取得 所有 <p> 元素
document.getElementById("the_id");              // 取得 id="the_id" 的元素
document.getElementsByClassName("class_name");  // 取得 class="class_name" 的元素
```

對應 jQuery 的版本：

```javascript
$("p");            // 代表取的是 <p> 元素
$("#the_id");      // # 字號代表後面接的是 id 的名稱
$(".class_name");  // . 符號代表後面接的是 class 的名稱
```

## 元素的內容

html：

```markup
<p>這是段落一</p>
```

JavaScript：

```javascript
var el_p = document.getElementsByTagName("p")[0]; // 取得元素
console.log( el_p.innerHTML ); // 取得「這是段落一」
```

對應 jQuery 的版本：

```javascript
console.log( $("p").html() ); // 取得「這是段落一」，預設會取得第一個 <p> 元素的內容
```

{% embed url="https://codepen.io/carlos411/pen/oNNZPWe" %}



## 元素的屬性

html：

```markup
<p id="para1" data-id="abcd1234">這是段落一</p>
```

JS：

```javascript
var el_p = document.getElementById("para1");
console.log( el_p.getAttribute("data-id") ); // abcd1234
```

jQuery：

```javascript
$(function(){
  console.log( $("#para1").attr("data-id") ); // abcd1234
});
```



例：

{% embed url="https://codepen.io/carlos411/pen/PoNwwGR" %}





## 表單欄位\(text\)

html：

```markup
<input type="text" id="the_text">
<button type="button" id="the_btn">取得值</button>
```

JavaScript：

```javascript
var el_the_btn = document.getElementById("the_btn");             // 取得 button 元素
el_the_btn.addEventListener("click", function(){                 // button 的 click 事件綁定
  var el_the_text = document.getElementById("the_text");         // 取得欄位元素
  console.log(el_the_text.value);                                // 取得值
});
```

jQuery：

```javascript
$("#the_btn").on("click", function(){
  console.log($("#the_text").val());
});
```

請測試看是否真的能取得到值。

## 表單欄位\(textarea\)

html：

```markup
<textarea id="the_textarea"></textarea>
<button type="button" id="the_btn">取得值</button>
```

JavaScript：

```javascript
var el_the_btn = document.getElementById("the_btn");
el_the_btn.addEventListener("click", function(){                 // button 的 click 事件綁定
  var el_the_textarea = document.getElementById("the_textarea");
  console.log(el_the_textarea.value);
});
```

jQuery：

```javascript
$("#the_btn").on("click", function(){
  console.log($("#the_textarea").val());
});
```

請測試看是否真的能取得到值。

## 表單欄位\(select\)

html：

```markup
<select id="the_select">
  <option value="1">選項一</option>
  <option value="2">選項二</option>
</select>
<button type="button" id="the_btn">取得值</button>
```

JavaScript：

```javascript
var el_the_btn = document.getElementById("the_btn");       // 取得 button 欄位

el_the_btn.addEventListener("click", function(){           // button 的 click 事件綁定
  var el_select = document.getElementById("the_select");   // 取得 select 下拉選單
  console.log(el_select.value);                            // 取得 select 目前所選的值，用 console.log 查看
});
```

jQuery：

```javascript
$("#the_btn").on("click", function(){
  console.log($("#the_select").val());
});
```

請測試看是否真的能取得到值。

## 表單欄位\(radio\)

html：

```markup
<input type="radio" name="food_type" value="1"> 葷
<input type="radio" name="food_type" value="2"> 素
<button type="button" id="the_btn">取得值</button>
```

JavaScript：

```javascript
var el_the_btn = document.getElementById("the_btn");            // 取得 button 欄位

el_the_btn.addEventListener("click", function(){                // button 的 click 事件綁定
  var el_input_radio = document.getElementsByTagName("input");  // 取的 input 欄位
  for(var i = 0; i < el_input_radio.length; i++){               // 使用 for 迴圈跑過每個 input 欄位
    if(el_input_radio[i].checked){                              // 如果是有選到的(.checked)
      console.log(el_input_radio[i].value)                      // 這裡可取得選到的那個選項的值(.value)
    }
  }
});
```

jQuery：

```javascript
$("#the_btn").on("click", function(){
  console.log( $('input[name=food_type]:checked').val() );  // 取得選到的那個選項的值
});
```

請測試看是否真的能取得到值。

## 表單欄位\(checkbox\)

html：

```markup
<input type="checkbox" name="habits" value="1"> 興趣1
<input type="checkbox" name="habits" value="2"> 興趣2
<button type="button" id="the_btn">取得值</button>
```

JavaScript：

```javascript
var el_the_btn = document.getElementById("the_btn");               // 取得 button 欄位

el_the_btn.addEventListener("click", function(){                   // button 的 click 事件綁定
  var el_input_checkbox = document.getElementsByTagName("input");  // 取的 input 欄位
  for(var i = 0; i < el_input_checkbox.length; i++){               // 使用 for 迴圈跑過每個 input 欄位
    if(el_input_checkbox[i].checked){                              // 如果是有選到的(.checked)
      console.log(el_input_checkbox[i].value)                      // 這裡可取得選到的那個選項的值(.value)
    }
  }
});
```

jQuery：

```javascript
$("#the_btn").on("click", function(){

  $('input[name=habits]').each(function(){
    if( $(this).prop("checked") ){          // this 就是每次迴圈，所代表的某個欄位。 .prop("checked") 表示有選到的話，回傳 true
      console.log($(this).val())            // 取得有選到的該 checkbox 的值
    }
  });

});
```

請測試看是否真的能取得到值。

