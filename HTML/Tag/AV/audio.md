# `<audio>标签`

`<audio>` 标签定义声音，比如音乐或其他音频流。

目前，`<audio>` 元素支持的3种文件格式：MP3、Wav、Ogg。

![image-20220719132000511](D:/Data/typora/photo/image-20220719132000511.png)

**提示：**可以在 `<audio>` 和 `</audio>` 之间放置文本内容，这些文本信息将会被显示在那些不支持 `<audio>` 标签的浏览器中。

**注意**：

- `<audio>` 标签是 HTML5 的新标签。
- 音视频文件引入时，默认情况下不允许用户自己控制播放停止。

**例**：

```html
<audio src="audio.mp3" controls></audio><!--是否允许用户控制播放-->
<audio src="audio.mp3" autoplay></audio><!--音频文件是否自动播放-->
<audio src="audio.mp3" loop></audio><!--音乐是否循环播放-->
```

## 浏览器支持

表格中的数字表示支持该标签的第一个浏览器版本号。

![image-20220719132141797](D:/Data/typora/photo/image-20220719132141797.png)

## 属性

(**New**) ：HTML5 中的新属性。

|                  属性                  |         值         |                            描述                             |
| :------------------------------------: | :----------------: | :---------------------------------------------------------: |
| [autoplay](audio_autoplay.md)(**New**) |      autoplay      |          如果出现该属性，则音频在就绪后马上播放。           |
| [controls](audio_controls.md)(**New**) |      controls      | 如果出现该属性，则向用户显示音频控件（比如播放/暂停按钮）。 |
|     [loop](audio_loop.md)(**New**)     |        loop        |       如果出现该属性，则每当音频结束时重新开始播放。        |
|    [muted](audio_muted.md)(**New**)    |       muted        |             如果出现该属性，则音频输出为静音。              |
|  [preload](audio_preload.md)(**New**)  | auto metadata none |    规定当网页加载时，音频是否默认被加载以及如何被加载。     |
|      [src](audio_src.md)(**New**)      |       *URL*        |                    规定音频文件的 URL。                     |

## 全局属性

`<audio>` 标签支持 HTML 的[全局属性](../../Appendix/global properties.md)。

## 事件属性

`<audio>` 标签支持 HTML 的[事件属性](../../Appendix/event properties.md)。
