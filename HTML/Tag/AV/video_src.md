# `<video>src属性`

src 属性指定 video 文件的本地路径(URL) 。

以上实例使用了 Ogg 文件, 该使用可正常显示于 Firefox, Opera 和 Chrome。

如果需要在 Internet Explorer 和 Safari 播放视频, 必须使用 MPEG4 文件。

如果想在所有浏览器播放视频文件 - 可在 `<video>` 元素总使用 [`<source>`](source.md)元素。 `<source>` 元素可以链接到不同的视频文件。浏览器将使用第一个可识别的格式：

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- 所有主流浏览器都支持 src 属性。但是定义的文件格式并不是所有浏览器都支持。
-  Internet Explorer 8 及更早IE版本不支持 `<video>` 标签。

**例**：

播放一个视频：

```html
<video src="movie.ogg" controls>
  您的浏览器不支持 video 标签。
</video>
```

## HTML 与 XHTML 之间的区别

在 XHTML中, 属性不允许简写，controls 属性必须定义为： `<video controls="controls">`。

------

## 语法

```html
<video src="URL">
```

## 属性值

|  值   |                             描述                             |
| :---: | :----------------------------------------------------------: |
| *URL* | 视频文件的 URL。可能的值：绝对 URL - 指向另一个站点（比如 `href="http://www.example.com/song.ogg"`）、相对 URL - 指向网站内的文件（比如 `href="song.ogg"`） |
