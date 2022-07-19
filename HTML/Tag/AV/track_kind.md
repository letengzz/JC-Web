# `<track>kind属性`

kind 属性规定轨道的种类。

**注意**：

- `<track>` 标签是 HTML5 中的新标签。
- Internet Explorer 10, Opera, 和 Chrome 支持 kind 属性。

**例**：

带有两个字幕轨道的 video 元素：

```html
<video width="320" height="240" controls>
  <source src="forrest_gump.mp4" type="video/mp4">
  <source src="forrest_gump.ogg" type="video/ogg">
  <track src="subtitles_en.vtt" kind="subtitles" srclang="en"
  label="English">
  <track src="subtitles_no.vtt" kind="subtitles" srclang="no"
  label="Norwegian">
</video>
```

## 语法

```html
<track src="subtitles_en.vtt" kind="subtitles" srclang="en">
```

## 属性值

|      值      |                             描述                             |
| :----------: | :----------------------------------------------------------: |
|   captions   |            该轨道定义将在播放器中显示的简短说明。            |
|   chapters   |              该轨道定义章节，用于导航媒介资源。              |
| descriptions | 该轨道定义描述，用于通过音频描述媒介的内容，假如内容不可播放或不可见。 |
|   metadata   |                  该轨道定义脚本使用的内容。                  |
|  subtitles   |            该轨道定义字幕，用于在视频中显示字幕。            |