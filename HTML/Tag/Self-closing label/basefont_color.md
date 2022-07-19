# `<basefont>color属性`

color 属性规定文档中文本的默认颜色。

**注意**：

- 只有 IE 9 和更早版本的 IE 浏览器支持 `<basefont>` 标签。应该避免使用该标签。
- HTML5 不支持 `<basefont>` 标签。请用 CSS 代替。
- 在 HTML 4.01 中，`<basefont>` 标签不支持任何事件属性。
- 使用 CSS 为文档中的文本规定**默认颜色、大小和字体**。

**例**：

指定页面上文本的默认字体颜色: 

```html
<head>
<basefont color="red" />
</head>

<body>
<h1>This is a header</h1>
<p>This is a paragraph</p>
</body>
```

## 兼容性注释

在 HTML 4.01 中，不赞成使用 basefont 元素的 color 属性；在 XHTML 1.0 Strict DTD 中，不支持 basefont 元素的 color 属性。

CSS 语法(在 `<head>` 部分): `<style>body{color:red}</style>`

[CSS：文本 color 属性的细节](../../../CSS/Property/Text/color.md)。

------

## 语法

```
<basefont color="color_name|hex_number|rgb_number" />
```

## 属性值

|      值      |                           描述                           |
| :----------: | :------------------------------------------------------: |
| *color_name* |      规定颜色值为颜色名称的字体颜色（比如 "red"）。      |
| *hex_number* |   规定颜色值为十六进制值的字体颜色（比如 "#ff0000"）。   |
| *rgb_number* | 规定颜色值为 rgb 代码的字体颜色（比如 "rgb(255,0,0)"）。 |
