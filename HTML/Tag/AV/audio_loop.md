# `<audio>loop属性`

loop 属性是一个布尔属性。

如果设置该属性，则音频将循环播放。

**注意**：

- `<audio>` 标签是 HTML 5 中的新标签。

**例**：

设置音频循环播放：

```html
<audio controls loop>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持 audio 元素。
</audio>
```

## 浏览器支持

Internet Explorer 9+, Firefox, Opera, Chrome, 和 Safari浏览器支持 loop属性。

**注意：** Internet Explorer 8 及更早版本不支持 `<audio>` 标签。

## HTML 与 XHTML之间的区别

在 XHTML 中, 该属性是不允许简写的 ， loop 属性必须定义为 `<audio loop="loop">`。

------

## 语法

```
<audio loop>
```

