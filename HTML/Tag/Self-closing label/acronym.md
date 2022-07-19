# `<acronym>标签`

`<acronym>` 标签定义首字母缩略词。

如果首字母缩略词是一个单词，则可以被读出来，例如 NATO, NASA, ASAP, GUI。

通过对只取首字母缩略词进行标记，您就能够为浏览器、拼写检查程序、翻译系统以及搜索引擎分度器提供有用的信息。

**注意**：

- 所有主流浏览器都支持 `<acronym>` 。
- IE 5.5 或更早版本的 IE 浏览器不支持 `<acronym>` 标签。
- HTML5 不支持 `<acronym>` 标签。请使用 [`<abbr>`](../Inline element/abbr.md) 标签代替它。HTML 4.01 支持 `<acronym>` 标签。
- 在某些浏览器中，当您把鼠标移至带有 `<acronym>` 标签的首字母缩略词上时，`<acronym>` 标签的 title 属性可被用来展示首字母缩略词的完整版本。

**例**：

被标记的首字母缩略词如下：

```html
Can I get this <acronym title="as soon as possible">ASAP</acronym>?
```

## 标准属性

在 HTML 4.01 中，`<acronym>` 标签支持如下标准属性：

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

## 事件属性

在 HTML 4.01 中，`<acronym>` 标签支持如下事件属性：

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

