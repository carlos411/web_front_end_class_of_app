# 2.12 表格 - &lt;table&gt;...&lt;/table&gt;

## 語意

即表格之意。

`<tr>`：**t**able **r**ow 的縮寫。

`<td>`：**t**able **d**ata 的縮寫。

`<th>`：**t**able **h**eading 的縮寫。

`<thead>`：**t**able **head** 的縮寫。

`<tfoot>`：**t**able **foot** 的縮寫。

`<tbody>`：**t**able **body** 的縮寫。

## 結構

基本結構 1

```html
<table>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
</table>
```

基本結構 2

```html
<table>
  <tr>
    <th></th>
    <th></th>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
</table>
```

進階結構

```html
<table>
  <thead>
    <tr>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td></td>
      <td></td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>
```

按照定義，`<tfoot>` 需緊接在 `<thead>` 之後，再來才是 `<tbody>`。

## 範例 1

```html
<table>
  <tr>
    <td>第一列第一欄</td>
    <td>第一列第二欄</td>
  </tr>
  <tr>
    <td>第二列第一欄</td>
    <td>第二列第二欄</td>
  </tr>
</table>
```

結果呈現

![](/assets/基本結構1.png)

## 範例 2

```html
<table>
  <tr>
    <td>第一列第一欄</td>
    <td>第一列第二欄</td>
  </tr>
  <tr>
    <td>第二列第一欄</td>
    <td>第二列第二欄</td>
  </tr>
</table>
```



