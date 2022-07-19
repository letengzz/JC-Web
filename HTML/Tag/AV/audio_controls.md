# `<audio>controls属性`

controls 属性是一个布尔属性。

如果属性存在，它指定音频控件的显示方式。

音视频控件包括：

- 播放
- 暂停
- 进度条
- 音量

**注意**：

- `<audio>` 元素是HTML5新增加的。

**例**：

带有浏览器默认控件的 `<audio>` 元素：

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持 audio 元素。
</audio>
```

## 浏览器支持

Internet Explorer 9+, Firefox, Opera, Chrome, 和 Safari浏览器支持 controls属性。

**注意：** Internet Explorer 8 及更早版本不支持 `<audio>` 标签。

## HTML 与 XHTML之间的区别

在 XHTML 中, 该属性是不允许简写的 ， controls 属性必须定义为 `<audio controls="controls">`。

------

## 语法

```
<audio controls>
```

