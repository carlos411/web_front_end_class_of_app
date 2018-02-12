# 2.1.1 宣告\(Declaration\)

~~HTML 4.01 Strict~~

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

~~XHTML 1.0 Strict~~

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

**HTML 5**

```html
<!DOCTYPE html>
```

# 2.1.2 標籤\(Tags\)

![](/assets/標籤.png)

# 2.1.3 屬性\(Attributes\)

![](/assets/屬性.png)

# 2.1.4 元素\(Elements\)

![](/assets/元素.png)

# 2.1.5 撰寫原則及基本觀念

* 所有標籤一律小寫。
* 多個連續空格，瀏覽器會視為只有一個空格。
* 避免有標籤交叉的狀況。例：`<p>這是文章段落，<div>另外</p>一段落。</div>`
* 縮排一律用 2 個空格或 4 個空格。
* &lt;html&gt; 標籤內只有 &lt;head&gt; 和 &lt;body&gt; 兩個標籤。
* `<html>` 是 `<head>` 及 `<body>` 的**父元素**；相反地，`<head>` 及 `<body>` 是 `<html>` 的**子元素**。

# 2.1.6 練習：第一個網頁

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

