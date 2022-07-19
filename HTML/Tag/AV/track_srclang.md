# `<track>srclang属性`

srclang 属性定义轨道的语言。

如果 kind 属性的值是 "subtitles"，则 srclang 属性是必需的。

**注意**：

- `<track>` 标签是 HTML5 中的新标签。
- Internet Explorer 10, Opera, 和 Chrom 支持 srclang 属性。

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

|       值        |                描述                |
| :-------------: | :--------------------------------: |
| *language_code* | 双字母的语言代码，规定轨道的语言。 |