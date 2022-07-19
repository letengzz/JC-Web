# `<frameset>标签`

rows 属性规定 `<frameset>` 中行的尺寸和数量。

每个框架的高度是在逗号分隔列表中的 rows 属性中规定。

**注释：**一旦规定了 rows 属性值的数量，就定义了 `<frameset>` 中行的数量。

**注意**：

- 所有主流浏览器都支持 rows 属性。
- HTML5 不支持 `<frameset>` 标签。

**例**：

一个三行框架：

```html
<frameset rows="25%,*,25%">
	<frame src="frame_a.htm">
	<frame src="frame_b.htm">
	<frame src="frame_c.htm">
</frameset>
```

## 语法

```html
<frameset rows="*pixels|%|*">
```

## 属性值

|    值    |                         描述                          |
| :------: | :---------------------------------------------------: |
| *pixels* | 规定行高度，以像素计（比如 "100px" 或者只是 "100"）。 |
|   *%*    |   规定行高度，以可用空间的百分比计（比如 "50%"）。    |
|    *     |          可用空间的剩余部分将会分配给该行。           |