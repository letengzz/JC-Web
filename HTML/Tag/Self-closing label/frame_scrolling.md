# `<frame>标签`

`<frame>` 标签定义 `<frameset>` 中的子窗口（框架）。

`<frameset>` 中的每个 `<frame>` 都可以设置不同的属性，比如 border、scrolling, noresize 等等。

**注释：**如果您希望验证包含框架的页面，请确保 [](https://www.runoob.com/tags/tag-doctype.html) 被设置为 "HTML Frameset DTD" 或者 "XHTML Frameset DTD" 。

[请用 CSS 代替](../../../CSS)。

## HTML 4.01 与 HTML5之间的差异

HTML5 不支持 <frame> 标签，HTML 4.01 支持 <frame> 标签。

------

## HTML 与 XHTML 之间的差异

在 HTML 中，<frame> 标签没有结束标签。在 XHTML 中，<frame> 标签必须被正确地关闭。

## 可选的属性

|                             属性                             |     值      |                            描述                            |
| :----------------------------------------------------------: | :---------: | :--------------------------------------------------------: |
| [frameborder](https://www.runoob.com/tags/att-frame-frameborder.html) |     0 1     |       **HTML5 不支持**。规定是否显示框架周围的边框。       |
| [longdesc](https://www.runoob.com/tags/att-frame-longdesc.html) |    *URL*    | **HTML5 不支持**。规定一个包含有关框架内容的长描述的页面。 |
| [marginheight](https://www.runoob.com/tags/att-frame-marginheight.html) |  *pixels*   |       **HTML5 不支持**。规定框架的上方和下方的边距。       |
| [marginwidth](https://www.runoob.com/tags/att-frame-marginwidth.html) |  *pixels*   |         HTML5 不支持。规定框架的左侧和右侧的边距。         |
|   [name](https://www.runoob.com/tags/att-frame-name.html)    |   *name*    |               HTML5 不支持。规定框架的名称。               |
| [noresize](https://www.runoob.com/tags/att-frame-noresize.html) |  noresize   |           HTML5 不支持。规定无法调整框架的大小。           |
| [scrolling](https://www.runoob.com/tags/att-frame-scrolling.html) | yes no auto |         HTML5 不支持。规定是否在框架中显示滚动条。         |
|    [src](https://www.runoob.com/tags/att-frame-src.html)     |    *URL*    |        HTML5 不支持。规定在框架中显示的文档的 URL。        |

------

## 标准属性

在 HTML 4.01 中，`<frame>` 标签支持如下标准属性：

| 属性  |         值         |        描述        |
| :---: | :----------------: | :----------------: |
| class |    *classname*     |   规定元素的类名   |
|  id   |        *id*        | 规定元素的唯一 id  |
| style | *style_definition* | 规定元素的行内样式 |
| title |       *text*       | 规定元素的额外信息 |

如需完整的描述，请访问[标准属性](../../Appendix/global properties.md)。

------

## 事件属性

根据 W3C 的标准，在 HTML 4.01 中，`<frame>` 标签不支持任何的事件属性。

但是，所有的浏览器都支持 onload 事件。

如需完整的描述，请访问[事件属性](../../Appendix/event properties.md)。
