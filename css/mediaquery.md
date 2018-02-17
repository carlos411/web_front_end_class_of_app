# 3.17 排版 - 媒體查詢\(Media Query\)

因為設備及瀏覽器的差異，故有時需要針對不同的螢幕寬度，來撰寫不同的 CSS。

媒體查詢都會 `@media` 來開頭。

## 範例一

當螢幕寬度大於等於 768px 時，`<a>` 的文字顏色會變成紅色。

```css
@media (min-width: 768px){
  a{
    color: red;
  }
}
```

## 範例二

當螢幕寬度小於等於 767px 時，`<a>` 的文字顏色會變成綠色。

```css
@media (max-width: 767px){
  a{
    color: green;
  }
}
```

## 範例三

當螢幕寬度大於等於 768px 且小於等於 992px 時，`<a>` 的文字顏色會變成橘色。

```css
@media (min-width: 768px) and (max-width: 992px){
  a{
    color: orange;
  }
}
```

## 範例四

* screen：會套用至彩色螢幕時。
* print：會套用至列印時。

在彩色螢幕上，`<a>` 的連結文字會是紫色；但列印時，會是藍色。

```css
@media screen{
  a{
    color: purple;
  }
}

@media print{
  a{
    color: blue;
  }
}
```

## 範例五

當是彩色螢幕時，螢幕寬度大於等於 768px 且小於等於 992px 時，`<a>` 的文字顏色會變成紅色。

```css
@media screen and (min-width: 768px) and (max-width: 992px){
  a{
    color: red;
  }
}
```

## 範例六

當是彩色螢幕時，且設備為橫向\(**landscape**\)擺放時，&lt;a&gt; 的文字顏色會是紅色；反之，若設備為直向\(**portrait**\)擺放時，會是藍色。

```css
@media screen and (orientation: landscape) {
  a{
    color: red;
  }
}

@media screen and (orientation: portrait) {
  a{
    color: blue;
  }
}
```



