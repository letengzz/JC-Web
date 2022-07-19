# `<audio>preload属性`

preload 属性规定是否在页面加载后载入音频。

如果设置了 autoplay 属性，则忽略该属性。

**注意**：

- preload 属性是 HTML 5 中的新属性。`<audio>` 标签是HTML5新标签。
- 目前所有主流浏览器都支持 preload 属性，除了 Internet Explorer。

**例**：

设置为预加载的 preload 元素：

```html
<audio controls preload="none">
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持 audio 元素。
</audio>
```

## 语法

```
<audio preload="auto|metadata|none">
```

## 属性值

|  值  |                             描述                             |
| :--: | :----------------------------------------------------------: |
| load | 规定是否预加载音频。可能的值：auto当页面加载后载入整个音频、meta 当页面加载后只载入元数据、none -当页面加载后不载入音频 |