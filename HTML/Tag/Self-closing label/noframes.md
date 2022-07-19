# `<noframes>标签`

`<noframes>` 元素可为那些不支持框架的浏览器显示文本。noframes 元素位于 frameset 元素内部。

`<noframes>` 元素插入在 `<frameset>` 元素中使用。

**注意**：

- HTML5 不支持 `<noframes>` 标签。
- 目前大多数浏览器支持 `<noframes>` 标签。

**例**：

显示三个frame框架，如果不支持frame输出 `<noframes>` 标签的文本：

```html
<html>

<frameset cols="25%,50%,25%">
  <frame src="frame_a.htm">
  <frame src="frame_b.htm">
  <frame src="frame_c.htm">
  <noframes>Sorry, your browser does not handle frames!</noframes>
</frameset>

</html>
```

## HTML 4.01 与 HTML5 的差异

HTML5不支持 `<noframes>` 标签，HTML 4.01 支持该标签。

------

## HTML 与 XHTML 的差异

**重要：** 在 XHTML Frameset DTD，位于 `<noframes>` 元素中的文本信息必须有关闭标签。

------

## 标准属性

在 HTML 4.01 中，`<noframes>` 支持如下标准属性：

|   属性   |         值         |                描述                 |
| :------: | :----------------: | :---------------------------------: |
|  class   |    *classname*     |           规定元素的类名            |
|   dir    |      rtl ltr       |      规定元素中内容的文本方向       |
|    id    |        *id*        |          规定元素的唯一 id          |
|   lang   |  *language_code*   |      规定元素中内容的语言代码       |
|  style   | *style_definition* |         规定元素的行内样式          |
|  title   |       *text*       |         规定元素的额外信息          |
| xml:lang |  *language_code*   | 规定 XHTML 文档中元素内容的语言代码 |

如需完整的描述，请访问[标准属性](../../Appendix/global properties.md)。

------

## 事件属性

在 HTML 4.01 中，`<noframes>` 标签支持如下事件属性：

|    属性     |    值    |                 描述                 |
| :---------: | :------: | :----------------------------------: |
|   onclick   | *script* |        当鼠标被单击时执行脚本        |
| ondblclick  | *script* |        当鼠标被双击时执行脚本        |
| onmousedown | *script* |      当鼠标按钮被按下时执行脚本      |
| onmousemove | *script* |       当鼠标指针移动时执行脚本       |
| onmouseout  | *script* |    当鼠标指针移出某元素时执行脚本    |
| onmouseover | *script* | 当鼠标指针悬停于某元素之上时执行脚本 |
|  onmouseup  | *script* |      当鼠标按钮被松开时执行脚本      |
|  onkeydown  | *script* |        当键盘被按下时执行脚本        |
| onkeypress  | *script* |    当键盘被按下后又松开时执行脚本    |
|   onkeyup   | *script* |        当键盘被松开时执行脚本        |

如需完整的描述，请访问[事件属性](../../Appendix/event properties.md)。