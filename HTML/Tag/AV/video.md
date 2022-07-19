# `<video>标签`

`<video>` 标签定义视频，比如电影片段或其他视频流。

目前，`<video>` 元素支持三种视频格式：MP4、WebM、Ogg。

|      浏览器       |                           MP4                           | WebM | Ogg  |
| :---------------: | :-----------------------------------------------------: | :--: | :--: |
| Internet Explorer |                           YES                           |  NO  |  NO  |
|      Chrome       |                           YES                           | YES  | YES  |
|      Firefox      | YES 从 Firefox 21 版本开始 Linux 系统从 Firefox 30 开始 | YES  | YES  |
|      Safari       |                           YES                           |  NO  |  NO  |
|       Opera       |                YES 从 Opera 25 版本开始                 | YES  | YES  |

- MP4 = MPEG 4文件使用 H264 视频编解码器和AAC音频编解码器
- WebM = WebM 文件使用 VP8 视频编解码器和 Vorbis 音频编解码器
- Ogg = Ogg 文件使用 Theora 视频编解码器和 Vorbis音频编解码器

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- 可以在 `<video>` 和 `</video>` 标签之间放置文本内容，这样不支持 `<video>` 元素的浏览器就可以显示出该标签的信息。可以在 `<video>` 和 `</video>` 标签之间放置文本内容，这样不支持 `<video>` 元素的浏览器就可以显示出该标签的信息。

**例**：

播放录像：

```html
<video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
    您的浏览器不支持 video 标签。
</video>
```

## 浏览器支持

表格中的数字表示支持该属性的第一个浏览器版本号。

![image-20220719145150164](D:/Data/typora/photo/image-20220719145150164.png)

## 视频格式的 MIME 类型

| 格式 | MIME-type  |
| :--: | :--------: |
| MP4  | video/mp4  |
| WebM | video/webm |
| Ogg  | video/ogg  |

## 可选属性

(**New**)：HTML5 中的新属性。

|                  属性                  |         值         |                             描述                             |
| :------------------------------------: | :----------------: | :----------------------------------------------------------: |
| [autoplay](video_autoplay.md)(**New**) |      autoplay      |           如果出现该属性，则视频在就绪后马上播放。           |
| [controls](video_controls.md)(**New**) |      controls      |       如果出现该属性，则向用户显示控件，比如播放按钮。       |
|   [height](video_height.md)(**New**)   |      *pixels*      |                    设置视频播放器的高度。                    |
|     [loop](video_loop.md)(**New**)     |        loop        |     如果出现该属性，则当媒介文件完成播放后再次开始播放。     |
|    [muted](video_muted.md)(**New**)    |       muted        |            如果出现该属性，视频的音频输出为静音。            |
|   [poster](video_poster.md)(**New**)   |       *URL*        |     规定视频正在下载时显示的图像，直到用户点击播放按钮。     |
|  [preload](video_preload.md)(**New**)  | auto metadata none | 如果出现该属性，则视频在页面加载时进行加载，并预备播放。如果使用 "autoplay"，则忽略该属性。 |
|      [src](video_src.md)(**New**)      |       *URL*        |                     要播放的视频的 URL。                     |
|    [width](video_width.md)(**New**)    |      *pixels*      |                    设置视频播放器的宽度。                    |

## 全局属性

`<video>` 标签支持 HTML 的[全局属性](../../Appendix/global properties.md)。

------

## 事件属性

`<video>` 标签支持 HTML 的[事件属性](../../Appendix/event properties.md)。
