# `<source>srcset属性`

srcset 属性用于不同情况下显示的图片 URL。

`<source>` 应用于 `<picture>` 标签时需要使用到该属性。

**注意**：

- `<source>` 标签是 HTML5 中的新标签。

**例**：

1. 在 `<picture>` 标签中使用 `<source>` 来设置不同屏幕显示的图片：

   ```html
   <picture>
     <source media="(min-width:650px)" srcset="https://static.com/images/runoob-logo.png">
     <source media="(min-width:465px)" srcset="https://static.com/images/code-icon-script.png">
     <img src="https://static.com/images/mix/hjkg_icon.png"  style="width:auto;">
   </picture>
   ```

## 浏览器支持

表格中的数字表示支持该标签的第一个浏览器版本号。

![image-20220719144119963](D:/Data/typora/photo/image-20220719144119963.png)

## 语法

```
<source srcset="URL">
```

## 属性值

|  值   |                             描述                             |
| :---: | :----------------------------------------------------------: |
| *URL* | 规定媒体文件的 URL。可能的值：绝对 URL - 指向另一个网站（比如 `href="https://www.runoob.com/horse.ogg"`）、相对 URL - 指向网站内的一个文件（比如 `href="horse.ogg"`） |
