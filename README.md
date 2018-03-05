# 1 簡介

網站前端開發，核心技術為 **HTML**、**CSS**、**JavaScript**，從這三個前端技術開始紮根，未來可應用至其他領域\(例：網頁動畫、元件、資料視覺化等\)。故 HTML、CSS、JavaScript 是網站開發中一切的基礎。

這三者分別代表的意義：

# 1.1 HTML = HyperText Markup Language

HTML 負責「**結構**」、「**語意**」。

「結構」做的好，對「排版」有幫助。

「語意」做的好，對「SEO」有幫助。

# 1.2 CSS = Cascading Style Sheets

CSS 負責網頁的「**外觀**」，包含了視覺風格、排版。

# 1.3 JS = JavaScript

JavaScript 負責「**行為**」，包含了使用者與網頁之間的互動操作。

# 1.4 練習：第一個網頁

檔案所在路徑：`簡介/`

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

## 完成

index.html 點兩下於瀏覽器中直接開啟。

