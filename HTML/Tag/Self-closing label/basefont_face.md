# `<basefont>face属性`

face 属性规定文档中文本的默认字体。

**注意**：

- 只有 IE 9 和更早版本的 IE 浏览器支持 `<basefont>` 标签。应该避免使用该标签。
- HTML5 不支持 `<basefont>` 标签。请用 CSS 代替。
- 在 HTML 4.01 中，`<basefont>` 标签不支持任何事件属性。
- 使用 CSS 为文档中的文本规定**默认颜色、大小和字体**。

**例**：

规定页面上的默认字体字体：

```html
<head>
<basefont face="courier, serif" />
</head>

<body>
<h1>This is a header</h1>
<p>This is a paragraph</p>
</body>
```

## 兼容性注释

在 HTML 4.01 中，不赞成使用 basefont 元素的 face 属性；在 XHTML 1.0 Strict DTD 中，不支持 basefont 元素的 face 属性。

CSS 语法(`<head>` 部分): `<style>body{font-family: courier, serif}</style>`

[CSS：font-family 属性的细节](../../../CSS/Property/Font/font-family.md)。

------

## 语法

```
<basefont face="font_family" />
```

## 属性值

| 值            | 描述                                                         |
| :------------ | :----------------------------------------------------------- |
| *font_family* | 规定文本的字体。如需规定若干字体的优先表，请使用逗号将字体名称分开（比如 <basefont face="verdana,arial,sans-serif" />）。**** |
