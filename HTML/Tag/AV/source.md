# `<source>标签`

`<source>` 标签为媒体元素（比如 `<video>` 和 `<audio>`）定义媒体资源。

`<source>` 标签允许您规定两个视频/音频文件供浏览器根据它对媒体类型或者编解码器的支持进行选择。

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

2. 在 `<video>` 标签中使用 `<source>` 来设置视频：

   ```html
   <video width="320" height="240" controls>   
   	<source src="movie.mp4" type="video/mp4">  
       <source src="movie.ogg" type="video/ogg">   
       Your browser does not support the video tag. 
   </video>
   ```

## 浏览器支持

表格中的数字表示支持该标签的第一个浏览器版本号。

![image-20220719141753174](D:/Data/typora/photo/image-20220719141753174.png)

## 属性

**New**：HTML5 中的新属性。

|              属性               |      值       |                             描述                             |
| :-----------------------------: | :-----------: | :----------------------------------------------------------: |
| [media](source_media.md)**New** | *media_query* |          规定媒体资源的类型，供浏览器决定是否下载。          |
|   [src](source_src.md)**New**   |     *URL*     |                     规定媒体文件的 URL。                     |
|     [type](source_type.md)      |  *MIME_type*  |                  规定媒体资源的 MIME 类型。                  |
|              sizes              |               |                不同页面布局设置不同图片大小。                |
|   [srcset](source_srcset.md)    |     *URL*     | `<source>` 应用于 `<picture>` 标签时需要使用到。指定在不同情况下使用的图像 URL。 |

## 全局属性

`<source>` 标签支持 [HTML 的全局属性](../../Appendix/global properties.md)。

------

## 事件属性

`<source>` 标签支持[HTML的事件属性](../../Appendix/event properties.md)。
