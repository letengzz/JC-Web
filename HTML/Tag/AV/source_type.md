# `<source>type属性`

type 属性规定媒体资源的 MIME 类型。

**注意**：

- `<source>` 标签是 HTML5 中的新标签。
- Internet Explorer 8 及之前的版本不支持 `<source>` 标签。
- Internet Explorer 9+、Firefox、Opera、Chrome 和 Safari 支持 type 属性。

**例**：

1. type 属性的使用：

   ```html
   <audio controls>
   	<source src="horse.ogg" type="audio/ogg">
   	<source src="horse.mp3" type="audio/mpeg">
   	您的浏览器不支持 audio 元素。
   </audio>
   ```

## 语法

```html
<source type="MIME_type">
```

## 属性值

|     值      |                             描述                             |
| :---------: | :----------------------------------------------------------: |
| *MIME_type* | 规定媒体资源的 MIME 类型。  常见的 MIME 类型： 视频：video/ogg、video/mp4、video/webm、音频：audio/ogg、audio/mpeg、请参阅 [IANA MIME 类型](http://www.iana.org/assignments/media-types/)，获得标准 MIME 类型的完整列表。 |
