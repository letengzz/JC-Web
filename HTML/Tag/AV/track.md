# `<track>标签`

`<track>` 标签为媒体元素（比如 `<audio>` and `<video>`）规定外部文本轨道，也就是字幕，字幕格式有 WebVTT 格式（.vtt 格式文件）。

这个元素用于规定字幕文件或其他包含文本的文件，当媒体播放时，这些文件是可见的。

**注意**：

- `<track>` 标签是 HTML5 中的新标签。

**例**：

带有字幕轨道（friday.vtt）的视频：

```html
<video width="320" height="240" controls>
<video controls
       src="/video/php/friday.mp4">
    <track default
           kind="captions"
           srclang="en"
           src="/video/php/friday.vtt" />
    抱歉，您的浏览器不支持嵌入视频！
</video>
</video>
```

## 浏览器支持

表格中的数字表示支持该标签的第一个浏览器版本号。

![image-20220719144514886](D:/Data/typora/photo/image-20220719144514886.png)

## 可选的属性

(**New**)：HTML5 中的新属性。

| 属性                                 | 值                                                | 描述                                                         |
| :----------------------------------- | :------------------------------------------------ | :----------------------------------------------------------- |
| [default](track_default.md)(**New**) | default                                           | 规定该轨道是默认的。如果用户没有选择任何轨道，则使用默认轨道。 |
| [kind](track_kind.md)(**New**)       | captions chapters descriptions metadata subtitles | 规定文本轨道的文本类型。                                     |
| [label](track_label.md)(**New**)     | *text*                                            | 规定文本轨道的标签和标题。                                   |
| [src](track_src.md)(**New**)         | *URL*                                             | 必需的。规定轨道文件的 URL。                                 |
| [srclang](track_srclang.md)(**New**) | *language_code*                                   | 规定轨道文本数据的语言。如果 kind 属性值是 "subtitles"，则该属性是必需的。 |

## 全局属性

`<track>` 标签支持 [HTML 的全局属性](../../Appendix/global properties.md)。

------

## 事件属性

`<track>` 标签支持 [HTML 的事件属性](../../Appendix/event properties.md)。