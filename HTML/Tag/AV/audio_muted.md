# `<audio>muted属性`

muted 属性属于逻辑属性。

如被设置，则规定视频输出应该被静音。

**注意**：

- `<audio>` 属性是 HTML 5 中的新属性。

**例**：

被静音频：:

```html
<audio controls muted>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持 audio 元素。
</audio>
```

## 浏览器支持

Internet Explorer 9+, Firefox, Opera, Chrome, 和 Safari浏览器支持 muted属性。

**注意：** Internet Explorer 8 及更早版本不支持 `<audio>` 标签。

## HTML 与 XHTML之间的区别

在 XHTML 中，不允许属性简写，muted 属性必须定义为 `<audio muted="muted">`。

------

## 语法

```
<audio muted>
```

