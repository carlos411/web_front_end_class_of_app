# 練習：第一個網頁

建立一個專案資料夾，資料夾名稱建議都用英文及底線來取名，該資料夾裡面要有以下幾個項目：

* css/
* fonts/
* images/
* js/
* index.html

編輯 index.html：

## 第一步：撰寫 html

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
  </head>
  <body>
    <h1>這是內文標題</h1>
  </body>
</html>
```

## 第二步：撰寫 CSS

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
    <style>
    h1{
      color: red;
    }
    </style>
  </head>
  <body>
    <h1>這是內文標題</h1>
  </body>
</html>
```

## 第三步：撰寫 JS

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>這是網頁標題</title>
    <style>
    h1{
      color: red;
    }
    </style>
  </head>
  <body>
    <h1>這是內文標題</h1>
    <script type="text/javascript">
      var h1 = document.getElementsByTagName("h1")[0];
      h1.addEventListener("click", function(){
        alert("open dialog");
      });
    </script>
  </body>
</html>
```

## 最後

index.html 點兩下於瀏覽器中直接開啟。

