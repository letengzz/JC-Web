# HTML

​	`HTML` (`Hypertext Markup Language`)**超文本标记语言**。
​	它负责网页的三个要素之中的**结构**。
​	`HTML`使用**标签**的的形式来标识网页中的不同组成部分。
​	所谓超文本指的是超链接，使用**超链接**可以让我们从一个页面跳转到另一个页面。

# 基础

## 定义文档类型

```html
<!DOCTYPE html>
```

​	`<!DOCTYPE>`声明位于文档中的最前面的位置，处于 `<html>` 标签之前。

​	`<!DOCTYPE>`声明不是一个`HTML`标签；它是用来告知 Web 浏览器页面使用了哪种`HTML`版本。

​	在 HTML 4.01 中，`<!DOCTYPE>` 声明需引用 `DTD` (文档类型声明)，因为 HTML 4.01 是基于`SGML` (`Standard Generalized Markup Language` 标准通用标记语言)。`DTD` 指定了标记语言的规则，确保了浏览器能够正确的渲染内容。

​	`HTML5` 不是基于 `SGML`，因此不要求引用`DTD`。

**提示：**总是给您的 HTML 文档添加 `<!DOCTYPE>` 声明，确保浏览器能够预先知道文档类型。

**注意**：

1. <!DOCTYPE> 标签没有结束标签。

2. `<!DOCTYPE>` 声明不区分大小写。

**常用的`DOCTYPE`声明** --> [Here](/DOCTYPE)

------

## 注释

​	`HTML`的注释，注释中的内容会被浏览器所忽略，不会在网页中直接显示，但是可以在源码中查看注释，注释用来对代码进行解释说明的。

```html
<!-- 注释 -->
```

**注意**：

	1. 开发中一定要养成良好的编写注释的习惯，注释要求简单明了注释还可以将一些不希望显示的内容隐藏。
	2. 注释不能嵌套。
	3. 所有主流浏览器都支持 `<!--...-->` 注释标签。
	4. `<!--...-->` 注释标签不支持任何[标准属性](/标准属性)。
	5. `<!--...-->` 注释标签不支持任何[事件属性](/事件属性)。

## 网页的基本结构



## 标签的属性

**属性**：在标签中(开始标签或自结束标签)中可以设置属性。

**注意**：

	1. 属性是一个**键值对**(`x=y`)。
	1. 







## 自结束标签

​	标签一般**成对出现**，但有一些自结束标签。

### img

```html
<img>
<img />
```

### input

```html
<input>
<input />
```

## 字符编码