# `<dir>compact标签`

compact 属性是一个 boolean（布尔）属性。

compact 属性规定列表呈现的效果比正常情况更小巧，这是通过减少行间距以及对列表进行缩进来实现的。

**注意**：

- 目前所有主流浏览器都不支持 compact 属性。
- `<dir>` 标签在HTML5中已不再支持。[请用 CSS 代替](../../../CSS)。
- `<dir>` 的 compact 属性在 HTML 4.01 中**已废弃**。

**例**：

在目录列表中使用 compact 属性：

```html
<dir compact>
  <li>html</li>
  <li>xhtml</li>
  <li>css</li>
</dir>
```

## 兼容性注释

`<dir>` 的 compact 属性在 HTML 4.01 中已废弃。请使用 CSS 替代。

CSS syntax: `<dir style="line-height: 80%">`

[CSS：line-height property属性的细节](../../../CSS/Property/Text/line-height.md)。

------

## HTML 与 XHTML之间的差别

在 XHTML 中, 属性不允许简写, compact 属性必须定义为: `<dir compact="compact">`。

------

## 语法

```html
<dir compact>
```

