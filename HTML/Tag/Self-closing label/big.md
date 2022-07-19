# `<big>标签`

`<big>` 标签用来制作更大的文本。

**注意**：

- HTML5 不支持 `<big>` 标签。[请用 CSS 代替](../../../CSS)。
- 所有主流浏览器都支持 `<big>` 标签。
- HTML5 不支持 `<big>` 标签，HTML 4.01 支持 `<big>` 标签。
- 浏览器显示包含在big元素中的文字时，其字体将比周围的文字大1号，直到上限7号字体。也就是说，如果文字已经是最大号字体，那么`<big>`标签将不起作用。
- 可以嵌套`<big>`标签使用，每一对`<big>`标签都可以使字体放大1号，直到上限7号字体。
- 对于那些不支持`<big>`标签的浏览器来说，它经常被解释成粗体。

**例**：

让文本比常规的字体大一号：

```html
<p><big>这个文本比较大。</big></p>
```

## 标准属性

在 HTML 4.01 中，`<big>` 标签支持如下标准属性：

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

在 HTML 4.01 中，`<big>` 标签支持如下事件属性：

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