# `<video>loop属性`

loop 属性是一个 boolean（布尔） 属性。

loop 属性规定当视频结束后将重新开始播放。

如果设置该属性，则视频将循环播放。

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- Internet Explorer 8 及更早IE版本不支持`<video>` 标签。
- 所有主流浏览器都支持 loop 属性。

**例**：

设置为循环播放的 video 元素：

```html
<video controls loop>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## HTML 与 XHTML 之间的区别

在 XHTML 中, 属性不允许简写， loop 属性必须定义为 `<video loop="loop">`。

------

## 语法

```html
<video loop>
```
