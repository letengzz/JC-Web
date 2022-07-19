# `<video>autoplay属性`

autoplay 属性是 boolean(布尔) 属性。

autoplay 属性规定一旦视频就绪马上开始播放。如果设置了该属性，视频将自动播放。

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- 所有主流浏览器都支持 autoplay 属性。
-  Internet Explorer 8 及更早IE版本不支持 `<video>` 标签。

**例**：

设置为自动播放的 video 元素：

```html
<video controls autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## HTML 与 XHTML之间的区别

在 XHTML 中, 属性不允许简写，autoplay 属性必须定义为： `<video autoplay="autoplay">`。

------

## 语法

```html
<video autoplay>
```

