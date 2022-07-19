# `<frame>marginheight属性`

marginheight 属性规定框架内容与框架的上方和下方之间的高度，以像素计。

**注意**：

- 所有主流浏览器都支持 marginheight 属性。
- HTML5 不支持 `<frame>` 标签。

**例**：

第一个框架的上边距和下边距是 50 像素，第二个框架的上边距和下边距是 0 像素：

```html
<frameset cols="50%,50%">
  <frame src="frame_a.htm" marginheight="50">
  <frame src="frame_b.htm" marginheight="0">
</frameset>
```

## 语法

```html
<frame marginheight="pixels">
```

## 属性值

|    值    |            描述            |
| :------: | :------------------------: |
| *pixels* | 规定框架的上边距和下边距。 |
