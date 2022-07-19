# `<track>label属性`

label 属性规定了文本轨迹的标题。

例如，当用户选择字幕轨道时，标题会显示出来。

**注意**：

- Internet Explorer 10, Opera, 和 Chrome 支持 label 属性。
- `<track>` 标签是 HTML5 新标签。

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
<track src="subtitles_en.vtt" kind="subtitles" srclang="en" label="English">
```

## 属性值

|   值    |       描述       |
| :-----: | :--------------: |
| *label* | 规定轨道的标题。 |