# `<video>preload属性`

preload 属性规定是否在页面加载后载入视频。

如果设置了 autoplay 属性，则忽略该属性。

**注意：** 如果使用 autoplay 属性 preload 将被忽略。

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- 除了Internet Explorer，所有主流浏览器都支持 preload 属性。

**例**：

页面加载时视频不应该被载入：

```html
<video controls preload="none">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## 语法

```html
<video preload="auto|metadata|none">
```

## 属性值

|    值    |                   描述                    |
| :------: | :---------------------------------------: |
|   auto   |  指示一旦页面加载，则开始加载音频/视频。  |
| metadata | 指示当页面加载后仅加载音频/视频的元数据。 |
|   none   |     指示页面加载后不应加载音频/视频。     |
