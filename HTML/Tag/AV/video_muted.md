# `<video>muted属性`

muted 属性是一个 boolean(布尔) 属性。

muted 属性设置或返回音频/视频是否应该被静音（关闭声音）。

**注意**：

- `<video>` 标签是 HTML5 的新标签。
-  Internet Explorer 9 及更早IE版本不支持`<video>` 的 muted 属性。
- Internet Explorer 10, Firefox, Opera, Chrome, 和 Safari 6 支持 muted 属性。

**例**：

关闭视频的声音：

```html
<video controls muted>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## HTML 与 XHTML 之间的区别

在 XHTML 中, 属性不允许简写， muted 属性必须定义为 `<video muted="muted">`。

## 语法

```html
<video muted>
```
