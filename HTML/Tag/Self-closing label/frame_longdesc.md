# `<frame>longdesc属性`

longdesc 属性规定指向一个页面的 URL，该页面包含有关框架内容的长描述。

**提示：**由于浏览器对 longdesc 属性的支持性非常差，没有必要使用该属性。如需为某个 frame 提供长描述（如果有必要的话），只要简单地创建一个指向描述页面的链接即可（该链接对任何人都是可见的）。

**注意**：

- 几乎所有的主流浏览器都不支持 longdesc 属性。
- HTML5 不支持 `<frame>` 标签。

**例**：

longdesc 属性指向了带有框架内容长描述的页面：

```html
<frameset cols="50%,50%">
  <frame src="frame_a.htm" longdesc="w3s.txt">
  <frame src="frame_b.htm">
</frameset>
```

## 语法

```html
<frame longdesc="URL">
```

## 属性值

|  值   |                             描述                             |
| :---: | :----------------------------------------------------------: |
| *URL* | 规定描述框架内容的页面的 URL。可能的值：绝对 URL - 指向另一个网站（比如 `longdesc="http://www.example.com/description.txt"`）相对 URL - 指向网站内的一个文件（比如 longdesc="description.txt"） |
