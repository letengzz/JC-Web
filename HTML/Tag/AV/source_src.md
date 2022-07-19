# `<source>src属性`

src 属性规定要播放的媒体文件的 URL。

**注意**：

- `<source>` 标签是 HTML5 中的新标签。
- Internet Explorer 9+、Firefox、Opera、Chrome 和 Safari 支持 src 属性。
- Internet Explorer 8 及之前的版本不支持 `<source>` 标签。

**例**：

1. 带有两个源文件的音频播放器。浏览器应该选择哪个文件（如果这两个源文件浏览器都支持）：

   ```html
   <audio controls>  
       <source src="horse.ogg" type="audio/ogg">  
       <source src="horse.mp3" type="audio/mpeg">
       您的浏览器不支持 audio 元素。
   </audio>
   ```

## 语法

```html
<source src="*URL">
```

## 属性值

|  值   |                             描述                             |
| :---: | :----------------------------------------------------------: |
| *URL* | 规定媒体文件的 URL。可能的值：绝对 URL - 指向另一个网站（比如 `href="http://www.example.com/horse.ogg"`）、相对 URL - 指向网站内的一个文件（比如 `href="horse.ogg"`） |
