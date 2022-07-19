# `<frameset>标签`

`<frameset>` 标签定义一个框架集。

`<frameset>` 元素被用来组织一个或者多个 [`<frame>`](frame.md) 元素。每个 `<frame>` 有各自独立的文档。

`<frameset>` 元素规定在框架集中存在多少列或多少行，以及每行每列占用的百分比/像素。

**注释：**如果您希望验证包含框架的页面，请确保 [<!DOCTYPE>](../DOCTYPE.md) 被设置为 "`HTML Frameset DTD`" 或者 "`XHTML Frameset DTD`" 。

HTML DOM 参考手册： [Frameset 对象](../../../JavaScript/HTML/frameset.md)

**例**：

1. 水平框架

   ```html
   <!DOCTYPE html>
   <html>
   
   <frameset rows="25%,*,25%">
     <frame src="frame_a.htm">
     <frame src="frame_b.htm">
     <frame src="frame_c.htm">
   </frameset>
   
   </html>
   ```

2. 混合结构框架

   ```html
   <!DOCTYPE html>
   <html>
   
   <frameset rows="50%,50%">
     <frame src="frame_a.htm">
     <frameset cols="25%,75%">
       <frame src="frame_b.htm">
       <frame src="frame_c.htm">
     </frameset>
   </frameset>
   
   </html>
   ```

3. 含有noresize="noresize"属性的框架

   ```html
   <!DOCTYPE html>
   <html>
   
   <frameset cols="50%,*,25%">
     <frame src="frame_a.htm" noresize="noresize">
     <frame src="frame_b.htm">
     <frame src="frame_c.htm">
   </frameset>
   
   </html>
   ```

4. 简单的三框架页面：

   ```html
   <frameset cols="25%,*,25%">
     <frame src="frame_a.htm">
     <frame src="frame_b.htm">
     <frame src="frame_c.htm">
   </frameset>
   ```

## HTML 与 XHTML 之间的差异

无。

------

## 可选的属性

|           属性           |     值     |                      描述                      |
| :----------------------: | :--------: | :--------------------------------------------: |
| [cols](frameset_cols.md) | pixels % * | **HTML5 不支持**。规定框架集中列的数目和尺寸。 |
| [rows](frameset_rows.md) | pixels % * | **HTML5 不支持**。规定框架集中行的数目和尺寸。 |

------

## 标准属性

在 HTML 4.01 中，`<frameset>` 标签支持如下标准属性：

| 属性  |         值         |        描述        |
| :---: | :----------------: | :----------------: |
| class |    *classname*     |   规定元素的类名   |
|  id   |        *id*        | 规定元素的唯一 id  |
| style | *style_definition* | 规定元素的行内样式 |
| title |       *text*       | 规定元素的额外信息 |

如需完整的描述，请访问[标准属性](../../Appendix/global properties.md)。

------

## 事件属性

在 HTML 4.01 中，`<frameset>` 标签支持如下事件属性：

|   属性   |    值    |          描述          |
| :------: | :------: | :--------------------: |
|  onload  | *script* | 当文档被载入时执行脚本 |
| onunload | *script* | 当文档被卸下时执行脚本 |

如需完整的描述，请访问[事件属性](../../Appendix/event properties.md)。