# `<frame>marginwidth属性`

marginwidth 属性规定框架内容与框架的左侧和右侧之间的高度，以像素计。

**注意**：

- 所有主流浏览器都支持 marginwidth 属性。
- HTML5 不支持 `<frame>` 标签。

**例**：

第一个框架的左边距和右边距是 50 像素，第二个框架的左边距和右边距是 0 像素：

```html
<frameset cols="50%,50%">
  <frame src="frame_a.htm" marginwidth="50">
  <frame src="frame_b.htm" marginwidth="0">
</frameset>
```

## 语法

```html
<frame marginwidth="pixels">
```

## 属性值

|    值    |            描述            |
| :------: | :------------------------: |
| *pixels* | 规定框架的左边距和右边距。 |
