# `<dir>标签`

`<dir>` 标签被用来定义目录列表。

**注意**：

- 所有主流浏览器都支持 `<dir>` 标签。
- HTML5 不支持 `<dir>` 标签。[请用 CSS 代替](../../../CSS)。
- 在 HTML 4.01 中，`<dir>` 元素 **已废弃**。

**例**：

```html
<dir>
  <li>html</li>
  <li>xhtml</li>
  <li>css</li>
</dir>
```

## 可选的属性

|           属性            |   值    |                             描述                             |
| :-----------------------: | :-----: | :----------------------------------------------------------: |
| [compact](dir_compact.md) | compact | **HTML5 不支持。HTML 4.01 已废弃**。 规定列表必须比常规状态小一号呈现。 |

------

## 标准属性

在 HTML 4.01 中，`<dir>` 标签支持如下标准属性：

| 属性  |         值         |           描述           |
| :---: | :----------------: | :----------------------: |
| class |    *classname*     |      规定元素的类名      |
|  dir  |      rtl ltr       | 规定元素中内容的文本方向 |
|  id   |        *id*        |    规定元素的唯一 id     |
| lang  |  *language_code*   | 规定元素中内容的语言代码 |
| style | *style_definition* |    规定元素的行内样式    |
| title |       *text*       |    规定元素的额外信息    |

如需完整的描述，请访问[标准属性](../../Appendix/global properties.md)。

------

## 事件属性

在 HTML 4.01 中，`<dir>` 标签支持如下事件属性：

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