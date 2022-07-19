# `<audio>src属性`

src 属性描述了音频文件的地址 (URL)。

Ogg 文件格式的音频，可以在 Firefox, Opera 和 Chrome 浏览器下播放。

如果需要在 Internet Explorer 和 Safari浏览器播放音频，必须使用 MP3 文件。

如果需要兼容所有浏览器 - 请在`<audio>` 元素中使用[`<source>`](source.md)元素 。 `<source>` 元素可以链接到不同的音频文件。浏览器将使用第一个可识别的音频文件格式。

**注意**：

-  Internet Explorer 8 及更早 IE 版本不支持 `<audio>` 标签。
- Internet Explorer 9+, Firefox, Opera, Chrome, 和 Safari 浏览器都支持 src 属性。 。但是不是有的浏览器都支持音频的文件格式。
- `<audio>` 标签是HTML5新增的。

**例**：

播放音频:

```html
<audio src="horse.ogg" controls>
您的浏览器不支持 audio 元素。
</audio>
```

## 语法

```
<audio src="URL">
```

## 属性值

|  值   |                             描述                             |
| :---: | :----------------------------------------------------------: |
| *URL* | 规定音频/视频来源的 URL。可能的值：绝对 URL - 指向另一个网站（比如 `src="http://example.com/movie.ogg"`）、相对 URL - 指向网站内的某个文件（比如 `src="/data/movie.ogg"`） |