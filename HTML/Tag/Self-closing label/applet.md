# `<applet>标签`

在 HTML 4.01 中，`<applet>` 元素**已废弃**。

`<applet>` 标签定义嵌入的 applet。

**注意**：

- 某些浏览器中依然存在对 `<applet>` 但是需要额外的插件和安装过程才能起作用。
- HTML5 不支持 `<applet>` 标签。请使用 [`<object>`](../programs/object.md) 标签代替它。
- 在 HTML 4.01 中，`<applet>` 标签不支持任何[事件属性](../../Appendix/event properties.md)。
- HTML5 不支持 `<applet>` 标签，HTML 4.01 已废弃 `<applet>` 标签。

**例**：

一个嵌入的 Java applet：

```HTML
<applet code="Bubbles.class" width="350" height="350">
Java applet that draws animated bubbles.
</applet>
```

## 必需的属性

|  属性  |   值   |                     描述                     |
| :----: | :----: | :------------------------------------------: |
|  code  | *URL*  |         规定 Java applet 的文件名。          |
| object | *name* | 规定了包含该 applet 的一系列版本的资源名称。 |

## 可选的属性

|   属性   |                  值                   |                    描述                    |
| :------: | :-----------------------------------: | :----------------------------------------: |
|  align   | left right top bottom middle baseline |   规定 applet 相对于周围元素的对齐方式。   |
|   alt    |                *text*                 |          规定 applet 的替换文本。          |
| archive  |                 *URL*                 |            规定档案文件的位置。            |
| codebase |                 *URL*                 | 规定 code 属性中指定的 applet 的基准 URL。 |
|  height  |               *pixels*                |            规定 applet 的高度。            |
|  hspace  |               *pixels*                |        定义围绕 applet 的水平间隔。        |
|   name   |                *name*                 |    定义 applet 的名称（用在脚本中的）。    |
|  vspace  |               *pixels*                |        定义围绕 applet 的垂直间隔。        |
|  width   |               *pixels*                |            规定 applet 的宽度。            |

------

## 标准属性

在 HTML 4.01 中，`<applet>` 标签支持如下标准属性：

| 属性  |         值         |        描述        |
| :---: | :----------------: | :----------------: |
| class |    *classname*     |   规定元素的类名   |
|  id   |        *id*        | 规定元素的唯一 id  |
| style | *style_definition* | 规定元素的行内样式 |
| title |       *text*       | 规定元素的额外信息 |

如需完整的描述，请访问[标准属性](../../Appendix/global properties.md)。