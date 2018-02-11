# 3.1 套用 CSS

套用 CSS，讓原來沒有任何外觀的 html，加上美麗的外觀，包含文字、版面佈局等等。主要常用的 CSS 套用方式有以下幾種：

## 方式一：行內套用

直接使用 style 屬性，加在 html 的標籤內。但因為這樣會使得 html 過於雜亂，建議少用。

```html
<p style="color: blue;">這是段落，使用 屬性 style 來改變文字樣式。</p>
```

## 方式二：嵌入套用

在 html 當中，寫在 `<style>...</style>` 之中。可以在頁面的任何地方出現，但建議一般會放在 `<head>...</head>` 之中，這樣在內容出現時，就會是已經套用的形式。

```css
<head>
  <style>
    p{
      color: blue;
    }
  </style>
</head>
```

## 方式三：外部套用

一般來說，html、css，會建議寫在各自的檔案，以讓 html 儘可能保持乾淨不雜亂。例：

* index.html
* index.css

**index.css** 的內容如下：

```

```



