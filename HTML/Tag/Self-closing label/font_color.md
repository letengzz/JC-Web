# `<font>color属性`

color 属性规定 `<font>` 元素中文本的颜色。

**注意**：

- HTML5 不支持 `<font>` 标签。[请用 CSS 代替](../../../CSS)。
- 所有主流浏览器都支持 color属性。
- HTML 4.01 已废弃 `<font>` 标签。

**例**：

规定文本的颜色：

```html
<font color="red">This is some text!</font>
```

## 兼容性注释

在 HTML 4.01 中，`<font>` 的 color 属性被废弃。请用 CSS 代替。

CSS 语法：`<p style="color:red">`

[CSS：文本 color 属性的细节](../../../CSS/Property/Text/color.md)。

## 语法

```html
<font color="color_name|hex_number|rgb_number">
```

## 属性值

|      值      |                           描述                           |
| :----------: | :------------------------------------------------------: |
| *color_name* |      规定颜色值为颜色名称的文本颜色（比如 "red"）。      |
| *hex_number* |   规定颜色值为十六进制值的文本颜色（比如 "#ff0000"）。   |
| *rgb_number* | 规定颜色值为 rgb 代码的文本颜色（比如 "rgb(255,0,0)"）。 |
