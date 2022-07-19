# `<video>controls属性`

controls 属性是一个 boolean(布尔) 属性。

controls 属性规定浏览器应该为视频提供播放控件。

如果设置了该属性，则规定不存在作者设置的脚本控件。

浏览器控件应该包括：

- 播放
- 暂停
- 定位
- 音量
- 全屏切换
- 字幕（如果可用）
- 音轨（如果可用）

**注意**：

- `<video>` 标签是 HTML5 的新标签。
- 所有主流浏览器都支持 controls 属性。
-  Internet Explorer 8 及更早IE版本不支持 `<video>` 标签。

**例**：

带有浏览器默认控件的 `<video>` 元素：

```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

## HTML 与 XHTML 之间的区别

在 XHTML中, 属性不允许简写，controls 属性必须定义为： `<video controls="controls">`。

## 语法

```html
<video controls>
```

