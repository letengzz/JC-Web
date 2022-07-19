# `<audio>autoplay属性`

autoplay 属性规定一旦音频就绪马上开始播放。

如果设置了该属性，音频将自动播放。

**注意**：

- autoplay 属性是 HTML 5 中的新属性。

**例**：

设置为自动播放的 audio 元素：

```html
<audio controls autoplay>  
	<source src="horse.ogg" type="audio/ogg">   
	<source src="horse.mp3" type="audio/mpeg">   
	您的浏览器不支持 audio 元素。 
</audio>
```

## 浏览器支持

Internet Explorer 9+, Firefox, Opera, Chrome, 和 Safari浏览器支持 autoplay 属性。

**注意：** Internet Explorer 8 及更早版本不支持 `<audio>` 标签。

## HTML 与 XHTML之间的区别

在 XHTML 中, 该属性是不允许简写的 ， autoplay 属性必须定义为 `<audio autoplay="autoplay">`。

------

## 语法

```
<audio autoplay>
```

