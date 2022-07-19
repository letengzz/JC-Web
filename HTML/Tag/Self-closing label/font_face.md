# `<font>face属性`

face 属性规定 `<font>` 元素中文本的字体。

**提示：**face 属性的值可以保存若干个字体名称作为备选。请把您最希望显示的字体放在字体列表的第一个，当第一个字体不可用时，使用后边的备选字体。您应该把一个通用的字体放在最后（serif、sans-serif、monospace、cursive 或 fantasy），以便在前面列举的字体都不可用时，浏览器可以在通用字体库中找到该字体。

**注意**：

- HTML5 不支持 `<font>` 标签。[请用 CSS 代替](../../../CSS)。
- 所有主流浏览器都支持 face 属性。
- HTML 4.01 已废弃 `<font>` 标签。

**例**：

规定文本的字体：

```html
<font face="verdana">This is some text!</font>
```

## 兼容性注释

在 HTML 4.01 中，`<font>` 的 face 属性被废弃。请用 CSS 代替。

CSS 语法：`<p style="font-family: verdana">`

[CSS：font-family 属性的细节](../../../CSS/Property/Font/font-family.md)。

------

## 语法

```html
<font face="font_family">
```

## 属性值

|      值       |                             描述                             |
| :-----------: | :----------------------------------------------------------: |
| *font_family* | 规定文本的字体。如需规定若干字体的优先表，请使用逗号分隔字体名称（比如 <font face="verdana,arial,sans-serif">）。 |
