# `<basefont>标签`

在 HTML 4.01 中，`<basefont>` 元素 **已废弃**。

`<basefont>` 标签定义文档中所有文本的默认颜色、大小和字体。

**注意**：

- 只有 IE 9 和更早版本的 IE 浏览器支持 `<basefont>` 标签。应该避免使用该标签。
- HTML5 不支持 `<basefont>` 标签。[请用 CSS 代替](../../../CSS)。
- 在 HTML 4.01 中，`<basefont>` 标签不支持任何事件属性。
- 使用 CSS 为文档中的文本规定**默认颜色、大小和字体**。

**例**：

规定页面上文本的默认颜色和大小：

```html
<head>
<basefont color="red" size="5" />
</head>

<body>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body>
```

## 可选的属性

|            属性            |      值       |                             描述                             |
| :------------------------: | :-----------: | :----------------------------------------------------------: |
| [color](basefont_color.md) |    *color*    | **HTML5 不支持。 HTML 4.01 已废弃**。 规定文档中文本的默认颜色。 |
|  [face](basefont_face.md)  | *font_family* | **HTML5 不支持。 HTML 4.01 已废弃**。 规定文档中文本的默认字体。 |
|  [size](basefont_size.md)  |   *number*    | **HTML5 不支持。 HTML 4.01 已废弃**。 规定文档中文本的默认大小。 |

------

## 标准属性

在 HTML 4.01 中，`<basefont>` 标签支持如下标准属性：

| 属性  |         值         |           描述           |
| :---: | :----------------: | :----------------------: |
| class |    *classname*     |      规定元素的类名      |
|  dir  |      rtl ltr       | 规定元素中内容的文本方向 |
|  id   |        *id*        |    规定元素的唯一 id     |
| lang  |  *language_code*   | 规定元素中内容的语言代码 |
| style | *style_definition* |    规定元素的行内样式    |
| title |       *text*       |    规定元素的额外信息    |

如需完整的描述，请访问[标准属性](../../Appendix/global properties.md)。
