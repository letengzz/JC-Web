# 基本结构

```html
<!DOCTYPE html>
<html>
    <head>
        
    </head>
    <body>
        
    </body>
</html>
```

# `<html>标签`

​	`HTML`的根标签(元素)，网页中的所有内容都要写在根元素里面。

```html
<html>
    
</html>
```

## `<head>标签`

​	`head`是网页的头部，`head`中的内容不会在网页中直接出现，主要用来帮助浏览器或搜索引擎来解析网页的。

**例**：[meta标签](Tag/Meta/meta.md)用来设置网页的元数据、[title标签](Tag/Basis/title.md)显示到浏览器的标题栏，判断网页的主要内容。

```html
<head>
    <meta charset = "utf-8"> <!-- 设置网页的字符集，避免乱码问题-->
    <title>网页的标题</title>
</head>定义关于文档的信息
```

## `<body>标签`

​	`body`是HTML的子元素，表示网页的主体，网页中所有的可见内容都应该写在`body`中。
