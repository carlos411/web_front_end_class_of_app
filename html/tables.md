# 2.12 表格 - &lt;table&gt;...&lt;/table&gt;

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



