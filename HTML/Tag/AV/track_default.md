# `<track>default属性`

default 属性是一个 boolean（布尔）属性。

如果使用 default 属性，则规定应该使用该轨道，假如用户没有选择其他轨道的话。

**注意**：

- Internet Explorer 10, Opera, 和 Chrome 支持 default 属性。
- `<track>` 标签是 HTML5 新标签。

**例**：

下面是一个 video 元素，其中的两个字幕之一是默认的：

```html
<video width="320" height="240" controls>
  <source src="forrest_gump.mp4" type="video/mp4">
  <source src="forrest_gump.ogg" type="video/ogg">
  <track src="subtitles_en.vtt" kind="subtitles" srclang="en"
  label="English" default>
  <track src="subtitles_no.vtt" kind="subtitles" srclang="no"
  label="Norwegian">
</video>
```

## HTML 与 XHTML之间的差异

在 XHTML 中, 属性不允许简介， default 属性必须定义为： `<track default="default" />`。

------

## 语法

```html 
<track src="subtitles_en.vtt" default>
```

