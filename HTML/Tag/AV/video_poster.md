# `<video>poster属性`

poster 属性指定视频下载时显示的图像，或者在用户点击播放按钮前显示的图像。

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- 所有主流浏览器都支持 poster 属性。
-  Internet Explorer 8 及更早IE版本不支持 `<video>` 标签。

**例**：

带有预览图的视频播放器：

```html
<video controls poster="/images/w3html5.gif">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## 语法

```html
<video poster="URL">
```

## 属性值

|  值   |                             描述                             |
| :---: | :----------------------------------------------------------: |
| *URL* | 指定图片文件的URL。可能值：绝对URL - 指向另外一个站点URL (如：`href="http://www.example.com/poster.jpg"`)、相对URL - 指向同个站点的URL (如： `href="poster.jpg"`) |
