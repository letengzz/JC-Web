# `<source>media属性`

media 属性指定媒体资源的类型（文件为什么样的媒体/设备进行了优化）。

浏览器使用该属性，以确定它是否可以播放该文件。如果它不能，它可以选择不下载文件。

**注意：**

- 该属性可接受多个值。
- 几乎所有的主流浏览器都不支持 media 属性。
- `<source>` 标签是 HTML5 中的新标签。

media 属性的使用：

```html
<source src="movie.ogg" type="video/ogg" media="screen and (min-width:320px)">
```

## 语法

```html
<source media="value">
```

## 可能的运算符

|  值  |         描述          |
| :--: | :-------------------: |
| and  | 规定一个 AND 运算符。 |
| not  | 规定一个 NOT 运算符。 |
|  ,   | 规定一个 OR 运算符。  |

## 设备

|     值     |                     描述                     |
| :--------: | :------------------------------------------: |
|    all     |            默认。适用于所有设备。            |
|   aural    |                 语音合成器。                 |
|  braille   |                盲文反馈装置。                |
|  handheld  |        手持设备（小屏幕、有限带宽）。        |
| projection |                   投影仪。                   |
|   print    |           打印预览模式/打印页面。            |
|   screen   |                 计算机屏幕。                 |
|    tty     | 电传打字机以及类似的使用等宽字符网格的媒体。 |
|     tv     | 电视机类型设备（低分辨率、有限的滚屏能力）。 |

## 值

|         值          |                             描述                             |
| :-----------------: | :----------------------------------------------------------: |
|        width        | 规定目标显示区域的宽度。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (min-width:500px)" |
|       height        | 规定目标显示区域的高度。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (max-height:700px)" |
|    device-width     | 规定目标显示器/纸张的宽度。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (device-width:500px)" |
|    device-height    | 规定目标显示器/纸张的高度。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (device-height:500px)" |
|     orientation     | 规定目标显示器/纸张的方向。 可能的值："portrait" 或 "landscape"。 例子：media="all and (orientation: landscape)" |
|    aspect-ratio     | 规定目标显示区域的宽度/高度比。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (aspect-ratio:16/9)" |
| device-aspect-ratio | 规定目标显示器/纸张的 device-width/device-height 比率。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (aspect-ratio:16/9)" |
|        color        | 规定目标显示器的 bits/color。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (color:3)" |
|     color-index     | 规定目标显示器可以处理的颜色数。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (min-color-index:256)" |
|     monochrome      | 规定单色帧缓冲中的 bits/pixel。 可使用 "min-" 和 "max-" 前缀。 例子：media="screen and (monochrome:2)" |
|     resolution      | 规定目标显示器/纸张的像素密度 (dpi 或 dpcm)。 可使用 "min-" 和 "max-" 前缀。 例子：media="print and (resolution:300dpi)" |
|        scan         | 规定 tv 显示器的扫描方式。 可能的值："progressive" 和 "interlace"。 例子：media="tv and (scan:interlace)" |
|        grid         | 规定输出设备是否是网格或位图。 可能的值："1" 为网格，否则为 "0"。 例子：media="handheld and (grid:1)" |
