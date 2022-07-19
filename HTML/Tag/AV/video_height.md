# `<video>height属性`

height 属性指定视频播放器的高度，以像素计。

**提示：** 规定视频的高度和宽度是一个好习惯。如果设置这些属性，在页面加载时会为视频预留出空间。如果没有设置这些属性，那么浏览器就无法预先确定视频的尺寸，这样就无法为视频保留合适的空间。结果是，在页面加载的过程中，其布局也会产生变化。

**注意：** 请勿通过 height 和 width 属性来缩放视频！通过 height 和 width 属性来缩小视频，只会迫使用户下载原始的视频（即使在页面上它看起来较小）。正确的方法是在网页上使用该视频前，使用软件对视频进行压缩。

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- Internet Explorer 8 及更早IE版本不支持 `<video>` 标签。
- 所有主流浏览器都支持 height 属性。

**例**：

具有指定高度和宽度的视频：

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## 语法

```html
<video height="pixels">
```

## 属性值

|    值    |                   描述                    |
| :------: | :---------------------------------------: |
| *pixels* | 以像素计的高度值（比如 "100px" 或 100）。 |
