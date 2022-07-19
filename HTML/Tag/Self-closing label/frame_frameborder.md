# `<frame>frameborder属性`

frameborder 属性规定是否显示框架周围的边框。

**提示：**出于实用性方面的原因，最好不用设置该属性，请使用 CSS 来应用 [边框样式和颜色](../../../CSS/Basis/border.md)。

**注意**：

- 所有主流浏览器都支持 frameborder 属性。
- HTML5 不支持 `<frame>` 标签。

**例**：

不带边框的双框架页面：

```html
<frameset cols="50%,50%">
  <frame src="frame_a.htm" frameborder="0">
  <frame src="frame_b.htm" frameborder="0">
</frameset>
```

## 语法

```html
<frame frameborder="1|0">
```

## 属性值

|  值  |       描述       |
| :--: | :--------------: |
|  1   | 有边框（默认）。 |
|  0   |     无边框。     |
