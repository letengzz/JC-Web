# CSS

`CSS`(`Cascading Style Sheets`)层叠样式表。网页实际上是一个多层的结构，通过CSS可以分别为网页的每一个层来设置样式，而最终我们能看到只是网页的最上边一层，总之一句话，`CSS`用来设置网页中元素的样式。

**基本语法**

```html
选择器 声明块
```

**选择器**，通过选择器可以选中页面中的指定元素
            比如 p 的作用就是选中页面中所有的p元素

**声明块**，通过声明块来指定要为元素设置的样式
            声明块由一个一个的声明组成
            声明是一个名值对结构
一个样式名对应一个样式值，名和值之间以`:`连接，以`;`结尾。

# 定义方式

## 内联样式

​	内联样式又叫行内样式，在标签内部通过`style属性`来设置元素的样式。
**问题**：

1. 使用内联样式，样式只能对一个标签生效
2. 如果希望影响到多个元素必须在每一个元素中都复制一遍

   并且当样式发生变化时，我们必须要一个一个的修改，非常的不方便

**注意**：开发时绝对不要使用内联样式。

**例**：-->[Here]()

```html
<p style="color:red; font-size: 60px;">少小离家老大回，乡音无改鬓毛衰</p>
<p style="color: red; font-size: 60px;">今天天气真不错！</p>
```

## 内部样式表

​	将样式编写到`head`中的`style标签`里。然后通过CSS的选择器来选中元素并为其设置各种样式。

​	相较于[内联样式](#内联样式)可以同时为多个标签设置样式，并且修改时只需要修改一处即可全部应用。

​	内部样式表更加方便对样式进行复用
**问题**：

​	我们的内部样式表只能对一个网页起作用，它里边的样式不能跨页面进行复用。

```html
<html>
	<head>
        <style>
        	p{
            	color: green;
            	font-size: 50px;
        	}
    	</style> 
    </head>
    <body>
        <p>
            你好
        </p>
    </body>
</html>
```

## 外部样式表

​	可以将CSS样式编写到一个外部的CSS文件中,然后通过`link标签`来引入外部的CSS文件。

​	外部样式表需要通过`link标签`进行引入，意味着只要想使用这些样式的网页都可以对其进行引用使样式可以在不同页面之间进行复用。

**优点**：将样式编写到外部的CSS文件中，可以使用到浏览器的缓存机制，从而加快网页的加载速度，提高用户的体验。

```html
<html>
    <head>
        <link rel="stylesheet" href="./style.css">
    </head>
    <body>
        <p>
            你好
        </p>
    </body>
    
</html>
```

# 注释

​	CSS中的注释，注释中的内容会自动被浏览器所忽略。

```css
/*
	注释
*/
```

# 选择器

## 常用选择器

### 元素选择器

**作用**：根据标签名来选中指定的元素
**语法**：

```css
标签名{}
```

**例**：-->[Here]()

```css
<style>
	p{
		color: red;
	}
	h1{
		color: green;
    }
</style>
```

### id选择器

**作用**：根据元素的id属性值选中一个元素
**语法**：

```css
#id属性值{}
```

**例**：-->[Here]()

```css
<style>
	#red{
		color: red;
	}
	#green{
		color: green;
    }
</style>
```

### 类选择器

**作用**：根据元素的class属性值选中一组元素
**语法**：

```css
.class属性值{}
```

**例**：-->[Here]()

```css
<style>
	.blue{
		color: blue;
	}
	.abc{
		font-size: 20px;
    }
</style>
```

### 通配选择器

**作用**：选中页面中的所有元素
**语法**:

```css
*{}
```

**例**：-->[Here]()

```css
<style>
	*{
		color: blue;
	}
</style>
```

## 复合选择器

### 交集选择器

**作用**：选中同时复合多个条件的元素
**语法**：

```css
选择器1选择器2选择器3选择器n{}
```

**注意**：
	交集选择器中如果有元素选择器，必须使用元素选择器开头

**例**：-->[Here]()

```css
<style>
	div.red{
		font-size: 30px;
	}
	.a.b.c{
		color: blue
	}
</style>
```

### 并集选择器

**作用**：同时选择多个选择器对应的元素
**语法**：

```css
选择器1,选择器2,选择器3,选择器n{}
```

**例**：-->[Here]()

```css
<style>
	#b1,.p1,h1,span,div.red{
		font-size: 30px;
	}
</style>
```

## 关系选择器

![image-20220206163706441](C:\Users\LetengZzz\AppData\Roaming\Typora\typora-user-images\image-20220206163706441.png)

### 子元素选择器

**作用**：选中指定父元素的指定子元素
**语法**：

```css
父元素>子元素{}
```

**例**：-->[Here]()

```css
<style>
	div.box > span{
		font-size: 30px;
	}
</style>
```

### 后代选择器

**作用**：选中指定元素内的指定后代元素
**语法**：

```css
祖先 后代
```

**例**：-->[Here]()

```css
<style>
	div span{
             color: skyblue
	}
</style>
```

### 兄弟选择器

**选择下一个兄弟**
**语法**：

```css
前一个 + 下一个
```

**例**：-->[Here]()

```css
<style>
	p + span{
          color: red;
	}
</style>
```

**选择下边所有的兄弟**
**语法**：

```css
兄 ~ 弟
```

**例**：-->[Here]()

```css
<style>
	p ~ span{
          color: red;
	}
</style>
```

## 属性选择器

**选择含有指定属性的元素**

**语法**：

```css
[属性名]
```

**例**：-->[Here]()

```css
<style>
	p[title]{
        color: red;
	}
</style>
<body>
	<p title="abc">这是一个p</p>
</body>
```

**选择含有指定属性和属性值的元素**

**语法**：

```css
[属性名=属性值] 
```

**例**：-->[Here]()

```css
<style>
	p[title=abc]{
        color: red;
	}
</style>
<body>
	<p title="abc">这是一个p</p>
</body>
```

**选择属性值以指定值开头的元素**

**语法**：

```css
[属性名^=属性值] 
```

**例**：-->[Here]()

```css
<style>
	p[title^=ab]{
        color: red;
	}
</style>
<body>
	<p title="abc">这是一个p</p>
</body>
```

**选择属性值以指定值结尾的元素**

**语法**：

```css
[属性名$=属性值] 
```

**例**：-->[Here]()

```css
<style>
	p[title$=bc]{
        color: red;
	}
</style>
<body>
	<p title="abc">这是一个p</p>
</body>
```

**选择属性值中含有某值的元素的元素**

**语法**：

```css
[属性名*=属性值] 
```

**例**：-->[Here]()

```css
<style>
	p[title*=b]{
        color: red;
	}
</style>
<body>
	<p title="abc">这是一个p</p>
</body>
```

## 伪类选择器

伪类（不存在的类，特殊的类）伪类用来描述一个元素的**特殊状态**

**比如**：第一个子元素、被点击的元素、鼠标移入的元素...

**伪类一般情况下都是使用:开头**

### 所有的子元素进行排序

​	第一个子元素：`:first-child`

​	最后一个子元素：`:last-child` 

​	选中第n个子元素：`:nth-child()` 

​	否定伪类：`:not()` 

**特殊值**：
	第n个 n的范围0到正无穷：`n`

​	选中偶数位的元素：`2n` 或 `even` 

​	选中奇数位的元素：`2n+1` 或 `odd` 

**例**：-->[Here]()

```css
<style>
	p,p:first-child{
        color: red;
	}
	p:last-child{
    	color:green;
	}
	p:nth-child(2){
    	color:yellow;
	}
	p:not(:nth-child(2)){
    	color:blue;
	}
</style>
<body>
	<ul>
		
	</ul>
</body>
```

### 同类型元素中进行排序

​	第一个子元素：`:first-of-type`

​	最后一个子元素：`:last-of-type` 

​	选中第n个子元素：`:nth-of-type()` 

**特殊值**：
	第n个 n的范围0到正无穷：`n`

​	选中偶数位的元素：`2n` 或 `even` 

​	选中奇数位的元素：`2n+1` 或 `odd` 

**例**：-->[Here]()

```css
<style>
	p:first-of-type{
        color: red;
	}
	p:last-of-type{
    	color:green;
	}
	p:nth-of-type(2){
    	color:yellow;
	}
</style>
<body>
	<p>这是一个p</p>
	<span>这是一个span</span>
	<p>这是一个p</p>
	<p>这是一个p</p>
	<p>这是一个p</p>
</body>
```

### `<a>标签`中的伪类

​	表示没访问过的链接： `:link` 

​	表示访问过的链接：`:visited` 
**注意**：由于隐私的原因，所以`visited`这个伪类只能修改链接的颜色
​	表示鼠标移入的状态：`:hover` 

​	表示鼠标点击：`:active` 

**例**：-->[Here]()

```
         */
​        a:link{
​            color: red;
​        }
​        a:visited{
​            color: orange; 
​            /* font-size: 50px;   */
​        }

​        /* 
​          
​         */
​         a:hover{
​             color: aqua;
​             font-size: 50px;
​         }

​         /*
​         
​         */
​         a:active{
​             color: yellowgreen;
​             
​         }
```

## 伪元素选择器

 **伪元素**：表示页面中一些特殊的并不真实的存在的元素（特殊的位置）
                伪元素使用 `::` 开头

​	表示第一个字母：`::first-letter` 
​    表示第一行：`::first-line` 
​    表示选中的内容：`::selection` 
​    元素的开始：`::before` 
​    元素的最后：`::after` 

**注意**：`before`和`after` 必须结合`content`属性来使用

**例**：-->[Here]()

```css

```

## 选择器的权重

**样式的冲突**
	当我们通过不同的选择器，选中相同的元素，并且为相同的样式设置不同的值时，此时就发生了样式的冲突。

​	发生样式冲突时，应用哪个样式由选择器的权重（优先级）决定：

**选择器的权重**
![image-20220207112126506](C:\Users\LetengZzz\AppData\Roaming\Typora\typora-user-images\image-20220207112126506.png)

​	比较优先级时，需要将所有的选择器的优先级进行相加计算，最后优先级越高，则越优先显示（分组选择器是单独计算的）

​	选择器的累加不会超过其最大的数量级，类选择器在高也不会超过id选择器

​	如果优先级计算后相同，此时则优先使用靠下的样式

​	可以在某一个样式的后边添加 `!important` ，则此时该样式会获取到最高的优先级，甚至超过内联样式
**注意**：在开发中这个玩意一定要慎用！

**例**：-->[Here]()

```css

```

# 盒子模型

盒模型、盒子模型、框模型(`box model`)：CSS将页面中的所有元素都设置为了一个矩形的盒子
将元素设置为矩形的盒子后，对页面的布局就变成将不同的盒子摆放到不同的位置

每一个盒子都由一下几个部分组成：

- [内容区(`content`)](#盒子模型/内容区)

- [内边距(`padding`)](#盒子模型/内边距)

- [边框(`border`)](#盒子模型/边框)

- [外边距(`margin`)](#盒子模型/外边距)

## 内容区

内容区(`content`)，元素中的所有的子元素和文本内容都在内容区中排列  

内容区的大小由`width` 和 `height`两个属性来设置

​	设置内容区的宽度：`width` 
​	设置内容区的高度：`height` 

**例**：-->[Here]()

```css

```

## 边框

边框(`border`)，边框属于盒子边缘，边框里边属于盒子内部，出了边框都是盒子的外部

边框的大小会影响到整个盒子的大小

要设置边框，需要至少设置三个样式：

**边框的宽度**：`border-width`
`border-width`可以用来指定四个方向的边框的宽度值的情况：

>  四个值：上 右 下 左
> 三个值：上 左右 下
> 两个值：上下 左右
> 一个值：上下左右

用来单独指定某一个边的宽度

> border-top-width    
> border-right-width
> border-bottom-width
> border-left-width                

**边框的颜色**：`border-color`

`border-color`用来指定边框的颜色，同样可以分别指定四个边的边框：

>  四个值：上 右 下 左
> 三个值：上 左右 下
> 两个值：上下 左右
> 一个值：上下左右

用来单独指定某一个边的颜色

> border-top-color    
> border-right-color
> border-bottom-color
> border-left-color      

**注意**：`border-color`也可以省略不写，如果省略了则自动使用`color`的颜色值。

**边框的样式**：`border-style` 

`border-style`指定边框的样式
	表示实线：`solid` 
    点状虚线：`dotted` 
    虚线：`dashed` 
    双线：`double` 

`border-style`用来指定边框的样式，同样可以分别指定四个边的边框：

>  四个值：上 右 下 左
> 三个值：上 左右 下
> 两个值：上下 左右
> 一个值：上下左右

用来单独指定某一个边的样式

> border-top-style  
> border-right-style
> border-bottom-style
> border-left-style    

`border-style`的默认值是`none` 表示没有边框。

**border简写属性**，通过该属性可以同时设置边框所有的相关样式，并且没有顺序要求

用来单独指定某一个边的样式

> border-top
> border-right
> border-bottom
> border-left

**例**：-->[Here]()

```

 border-width: 10px; 
                
border-width: 10px; */
             /* border-top-width: 10px;
             border-left-width: 30px;

      border-color: orange red yellow green;
             border-color: orange; 
   

                  
       border-style: solid dotted dashed double;
             border-style: solid; */

             /* border-width: 10px;
             border-color: orange;
             border-style: solid;
           
              */
              /* border: solid 10px orange; */
              /* border-top: 10px solid red;
              border-left: 10px solid red;
              border-bottom: 10px solid red; */
```

## 内边框

内边距(`padding`)：内容区和边框之间的距离是内边距

内边距的设置会影响到盒子的大小

盒子的可见框的大小，由内容区 内边距 和 边框共同决定，所以在计算盒子大小时，需要将这三个区域加到一起计算

padding 内边距的简写属性，可以同时指定四个方向的内边距：

> padding-top
> padding-right
> padding-bottom
> padding-left

**例**：-->[Here]()

```css
              */
              padding: 10px 20px 30px 40px;
              padding: 10px 20px 30px ;
              padding: 10px 20px ;
              padding: 10px ;
​                      /* padding-top: 100px;
​             padding-left: 100px;
​             padding-right: 100px;
​             padding-bottom: 100px; */

​             /* 
```

## 外边框

 外边距(`margin`)：外边距不会影响盒子可见框的大小

一共有四个方向的外边距：

​	**上外边距**，设置一个正值，元素会向下移动：`margin-top`

​	**下外边距**，设置一个正值，其下边的元素会向下移动：**margin-bottom**

​	**左外边距**，设置一个正值，元素会向右移动：**margin-left**

​	**右外边距**，默认情况下设置margin-right不会产生任何效果：**margin-right**

`margin`也可以设置负值，如果是负值则元素会向相反的方向移动

**注意**：

1. 元素在页面中是按照自左向右的顺序排列的，所以默认情况下如果我们设置的左和上外边距则会移动元素自身，而设置下和右外边距会移动其他元素。

2. `margin`会影响到盒子实际占用空间。

**`margin`的简写属性**：
`margin`可以同时设置四个方向的外边距 ，用法和`padding`一样

**例**：-->[Here]()

```

             /* margin-top: 100px;
             margin-left: 100px;
             margin-bottom: 100px; */

             /* margin-bottom: 100px; */
             /* margin-top: -100px; */
             /* margin-left: -100px; */
             /* margin-bottom: -100px; */

             /* margin-right: 0px; */

             margin: 100px;
```

## 盒子的水平布局

元素在其父元素中水平方向的位置由以下几个属性共同决定“
                    `margin-left`
                    `border-left`
                    `padding-left`
                    `width`
                    `padding-right`
                    `border-right`
                    `margin-right`

一个元素在其父元素中，水平布局必须要满足以下的等式：

![image-20220212193146912](C:\Users\LetengZzz\AppData\Roaming\Typora\typora-user-images\image-20220212193146912.png)

**以上等式必须满足，如果相加结果使等式不成立，则称为过度约束，则等式会自动调整**

调整的情况：

​	如果这七个值中没有为`auto`的情况，则浏览器会自动调整`margin-right`值以使等式满足。

​	这七个值中有三个值和设置为`auto`

> ​	width
> ​	margin-left
> ​	margin-right

如果某个值为`auto`，则会自动调整为`auto`的那个值以使等式成立

`width`的值默认就是`auto`

```
0 + 0 + 0 + auto + 0 + 0 + 0 = 800  auto = 800
0 + 0 + 0 + auto + 0 + 0 + 200 = 800  auto = 600
200 + 0 + 0 + auto + 0 + 0 + 200 = 800  auto = 400

auto + 0 + 0 + 200 + 0 + 0 + 200 = 800  auto = 400


​                            auto + 0 + 0 + 200 + 0 + 0 + auto = 800  auto = 300
```

如果将一个宽度和一个外边距设置为`auto`，则宽度会调整到最大，设置为`auto`的外边距会自动为0

如果将三个值都设置为`auto`，则外边距都是0，宽度最大

如果将两个外边距设置为`auto`，宽度固定值，则会将外边距设置为相同的值

所以我们经常利用这个特点来使一个元素在其父元素中水平居中

```
        .inner{
            /* width: auto;  width的值默认就是auto*/
            width: 200px;
            height: 200px;
            background-color: #bfa;
            margin-right: auto;
            margin-left: auto;
            /* margin-left: 100px;
            margin-right: 400px */
            /* 


                    
margin-left+border-left+padding-left+width+padding-right+border-right+margin-right = 其父元素内容区的宽度 （必须满足）

                0 + 0 + 0 + 200 + 0 + 0 + 0 = 800
                0 + 0 + 0 + 200 + 0 + 0 + 600 = 800


                100 + 0 + 0 + 200 + 0 + 0 + 400 = 800
                100 + 0 + 0 + 200 + 0 + 0 + 500 = 800
                    - 
                            示例：
                                width:xxxpx;
                                margin:0 auto;



             */
        }
```

**例**：-->[Here]()

## 盒子的垂直布局

```
  .outer{
            background-color: #bfa;
            height: 600px;
            /* 
                默认情况下父元素的高度被内容撑开
             */
        }

        .inner{
            width: 100px;
            background-color: yellow;
            height: 100px;
            margin-bottom: 100px;
            
        }

        .box1{
            width: 200px;
            height: 200px;
            background-color: #bfa;
            /* 
                子元素是在父元素的内容区中排列的，
                    如果子元素的大小超过了父元素，则子元素会从父元素中溢出
                    使用 overflow 属性来设置父元素如何处理溢出的子元素

                    可选值：
                        visible，默认值 子元素会从父元素中溢出，在父元素外部的位置显示
                        hidden 溢出内容将会被裁剪不会显示
                        scroll 生成两个滚动条，通过滚动条来查看完整的内容
                        auto 根据需要生成滚动条

                overflow-x: 
                overflow-y:
             */
            overflow: auto;

            
        }

        .box2{
            width: 100px;
            height: 400px;
            background-color: orange;
        }
    
```

**例**：-->[Here]()

## 垂直外边距的折叠

相邻的垂直方向外边距会发生重叠现象

兄弟元素间的相邻垂直外边距会取两者之间的较大值（两者都是正值）

特殊情况：
如果相邻的外边距一正一负，则取两者的和
如果相邻的外边距都是负值，则取两者中绝对值较大的

兄弟元素之间的外边距的重叠，对于开发是有利的，所以我们不需要进行处理

父子元素

父子元素间相邻外边距，子元素的会传递给父元素（上外边距）

父子外边距的折叠会影响到页面的布局，必须要进行处理

**例**：-->[Here]()

## 行内元素的盒模型

```
      行内元素的盒模型
                    - 行内元素不支持设置宽度和高度
                    - 行内元素可以设置padding，但是垂直方向padding不会影响页面的布局
                    - 行内元素可以设置border，垂直方向的border不会影响页面的布局
                    - 行内元素可以设置margin，垂直方向的margin不会影响布局
             */
             /* width: 100px;
             height: 100px; */

             /* padding: 100px; */

             /* border: 100px solid red; */

             margin: 100px;
```

**例**：-->[Here]()

## 默认样式

```
 默认样式：
                - 通常情况，浏览器都会为元素设置一些默认样式
                - 默认样式的存在会影响到页面的布局，
                    通常情况下编写网页时必须要去除浏览器的默认样式（PC端的页面）
      
       重置样式表：专门用来对浏览器的样式进行重置的
            reset.css 直接去除了浏览器的默认样式
            normalize.css 对默认样式进行了统一
```

**例**：-->[Here]()

## 盒子的尺寸

```
                默认情况下，盒子可见框的大小由内容区、内边距和边框共同决定

                    box-sizing 用来设置盒子尺寸的计算方式（设置width和height的作用）
                        可选值：
                            content-box 默认值，宽度和高度用来设置内容区的大小
                            border-box 宽度和高度用来设置整个盒子可见框的大小
                                width 和 height 指的是内容区 和 内边距 和 边框的总大小
             */
            
            box-sizing: border-box;
```

**例**：-->[Here]()



# 浮动

```
通过浮动可以使一个元素向其父元素的左侧或右侧移动
                    使用 float 属性来设置于元素的浮动
                        可选值：
                            none 默认值 ，元素不浮动
                            left 元素向左浮动
                            right 元素向右浮动

                    注意，元素设置浮动以后，水平布局的等式便不需要强制成立
                        元素设置浮动以后，会完全从文档流中脱离，不再占用文档流的位置，
                            所以元素下边的还在文档流中的元素会自动向上移动

                    浮动的特点：
                        1、浮动元素会完全脱离文档流，不再占据文档流中的位置
                        2、设置浮动以后元素会向父元素的左侧或右侧移动，
                        3、浮动元素默认不会从父元素中移出
                        4、浮动元素向左或向右移动时，不会超过它前边的其他浮动元素
                        5、如果浮动元素的上边是一个没有浮动的块元素，则浮动元素无法上移
                        6、浮动元素不会超过它上边的浮动的兄弟元素，最多最多就是和它一样高

                    简单总结：
                        浮动目前来讲它的主要作用就是让页面中的元素可以水平排列，
                            通过浮动可以制作一些水平方向的布局     浮动元素不会盖住文字，文字会自动环绕在浮动元素的周围，
                    所以我们可以利用浮动来设置文字环绕图片的效果
                       元素设置浮动以后，将会从文档流中脱离，从文档流中脱离后，元素的一些特点也会发生变化

                脱离文档流的特点：
                    块元素：
                        1、块元素不在独占页面的一行
                        2、脱离文档流以后，块元素的宽度和高度默认都被内容撑开

                    行内元素：
                        行内元素脱离文档流以后会变成块元素，特点和块元素一样

                    脱离文档流以后，不需要再区分块和行内了 
```



## 高度塌陷问题

```
 BFC(Block Formatting Context) 块级格式化环境
                    - BFC是一个CSS中的一个隐含的属性，可以为一个元素开启BFC
                        开启BFC该元素会变成一个独立的布局区域
                    - 元素开启BFC后的特点：
                        1.开启BFC的元素不会被浮动元素所覆盖
                        2.开启BFC的元素子元素和父元素外边距不会重叠
                        3.开启BFC的元素可以包含浮动的子元素

                    - 可以通过一些特殊方式来开启元素的BFC：
                        1、设置元素的浮动（不推荐）
                        2、将元素设置为行内块元素（不推荐）
                        3、将元素的overflow设置为一个非visible的值
                            - 常用的方式 为元素设置 overflow:hidden 开启其BFC 以使其可以包含浮动元素
     高度塌陷的问题：
                    在浮动布局中，父元素的高度默认是被子元素撑开的，
                        当子元素浮动后，其会完全脱离文档流，子元素从文档流中脱离
                        将会无法撑起父元素的高度，导致父元素的高度丢失

                    父元素高度丢失以后，其下的元素会自动上移，导致页面的布局混乱

                    所以高度塌陷是浮动布局中比较常见的一个问题，这个问题我们必须要进行处理！
                    
```

**例**：-->[Here]()

## 清除浮动问题

```
 由于box1的浮动，导致box3位置上移
                    也就是box3收到了box1浮动的影响，位置发生了改变

                如果我们不希望某个元素因为其他元素浮动的影响而改变位置，
                    可以通过clear属性来清除浮动元素对当前元素所产生的影响

                clear
                    - 作用：清除浮动元素对当前元素所产生的影响
                    - 可选值：
                        left 清除左侧浮动元素对当前元素的影响
                        right 清除右侧浮动元素对当前元素的影响
                        both 清除两侧中最大影响的那侧

                    原理：
                        设置清除浮动以后，浏览器会自动为元素添加一个上外边距，
                            以使其位置不受其他元素的影响
                            
```

**例**：-->[Here]()

## clearfix

```
/* clearfix 这个样式可以同时解决高度塌陷和外边距重叠的问题，当你在遇到这些问题时，直接使用clearfix这个类即可 */
        .clearfix::before,
        .clearfix::after{
            content: '';
            display: table;
            clear: both;
        }
```



# 定位

```
   定位（position）
                    - 定位是一种更加高级的布局手段
                    - 通过定位可以将元素摆放到页面的任意位置
                    - 使用position属性来设置定位
                        可选值：
                            static 默认值，元素是静止的没有开启定位
                            relative 开启元素的相对定位
                            absolute 开启元素的绝对定位
                            fixed 开启元素的固定定位
                            sticky 开启元素的粘滞定位

                    - 相对定位：
                        - 当元素的position属性值设置为relative时则开启了元素的相对定位
                        - 相对定位的特点：
                            1.元素开启相对定位以后，如果不设置偏移量元素不会发生任何的变化
                            2.相对定位是参照于元素在文档流中的位置进行定位的
                            3.相对定位会提升元素的层级
                            4.相对定位不会使元素脱离文档流
                            5.相对定位不会改变元素的性质块还是块，行内还是行内

                    - 偏移量（offset）
                        - 当元素开启了定位以后，可以通过偏移量来设置元素的位置
                            top
                                - 定位元素和定位位置上边的距离
                            bottom
                                - 定位元素和定位位置下边的距离

                                - 定位元素垂直方向的位置由top和bottom两个属性来控制
                                    通常情况下我们只会使用其中一
                                - top值越大，定位元素越向下移动
                                - bottom值越大，定位元素越向上移动
                            left
                                - 定位元素和定位位置的左侧距离
                            right
                                - 定位元素和定位位置的右侧距离

                                - 定位元素水平方向的位置由left和right两个属性控制
                                    通常情况下只会使用一个
                                - left越大元素越靠右
                                - right越大元素越靠左
```



## 绝对定位

```
  绝对定位
                - 当元素的position属性值设置为absolute时，则开启了元素的绝对定位
                - 绝对定位的特点：
                    1.开启绝对定位后，如果不设置偏移量元素的位置不会发生变化
                    2.开启绝对定位后，元素会从文档流中脱离
                    3.绝对定位会改变元素的性质，行内变成块，块的宽高被内容撑开
                    4.绝对定位会使元素提升一个层级
                    5.绝对定位元素是相对于其包含块进行定位的

                    包含块( containing block )
                        - 正常情况下：
                            包含块就是离当前元素最近的祖先块元素
                            <div> <div></div> </div>
                            <div><span><em>hello</em></span></div>

                        - 绝对定位的包含块:
                            包含块就是离它最近的开启了定位的祖先元素，
                                如果所有的祖先元素都没有开启定位则根元素就是它的包含块

                        - html（根元素、初始包含块）
```

**例**：-->[Here]()

## 固定定位

```

                固定定位：
                    - 将元素的position属性设置为fixed则开启了元素的固定定位
                    - 固定定位也是一种绝对定位，所以固定定位的大部分特点都和绝对定位一样
                        唯一不同的是固定定位永远参照于浏览器的视口进行定位
                        固定定位的元素不会随网页的滚动条滚动
```

**例**：-->[Here]()

## 粘滞定位

```
 粘滞定位
                    - 当元素的position属性设置为sticky时则开启了元素的粘滞定位
                    - 粘滞定位和相对定位的特点基本一致，
                        不同的是粘滞定位可以在元素到达某个位置时将其固定
```

**例**：-->[Here]()

## 绝对定位元素的布局

```
  水平布局
                    left + margin-left + border-left + padding-left + width + padding-right + border-right + margin-right + right = 包含块的内容区的宽度

                - 当我们开启了绝对定位后:
                    水平方向的布局等式就需要添加left 和 right 两个值
                        此时规则和之前一样只是多添加了两个值：
                            当发生过度约束：
                                如果9个值中没有 auto 则自动调整right值以使等式满足
                                如果有auto，则自动调整auto的值以使等式满足

                        - 可设置auto的值
                            margin width left right

                        - 因为left 和 right的值默认是auto，所以如果不指定left和right
                            则等式不满足时，会自动调整这两个值

                    垂直方向布局的等式的也必须要满足
                        top + margin-top/bottom + padding-top/bottom + border-top/bottom + height = 包含块的高度

            
```

**例**：-->[Here]()

## 元素的层级

```
对于开启了定位元素，可以通过z-index属性来指定元素的层级
                    z-index需要一个整数作为参数，值越大元素的层级越高
                        元素的层级越高越优先显示

                    如果元素的层级一样，则优先显示靠下的元素

                    祖先的元素的层级再高也不会盖住后代元素
             */
             /* z-index: 3; */
```

**例**：-->[Here]()

# 弹性盒子

**例**：-->[Here]()

# 声明块

## 轮廓和圆角

```
    <style>
        .box1{
            width: 200px;
            height: 200px;
            background-color: #bfa;

            /* box-shadow 用来设置元素的阴影效果，阴影不会影响页面布局 
                第一个值 水平偏移量 设置阴影的水平位置 正值向右移动 负值向左移动
                第二个值 垂直偏移量 设置阴影的水平位置 正值向下移动 负值向上移动
                第三个值 阴影的模糊半径
                第四个值 阴影的颜色
            */

            box-shadow: 0px 0px 50px rgba(0, 0, 0, .3) ; 

/* 

            outline 用来设置元素的轮廓线，用法和border一模一样
                轮廓和边框不同的点，就是轮廓不会影响到可见框的大小    
 */
            
        }

        /* .box1:hover{
            outline: 10px red solid;
        } */

        .box2{
            width: 200px;
            height: 200px;
            background-color: orange;

            /* border-radius: 用来设置圆角 圆角设置的圆的半径大小*/

            /* border-top-left-radius:  */
            /* border-top-right-radius */
            /* border-bottom-left-radius:  */
            /* border-bottom-right-radius:  */
            /* border-top-left-radius:50px 100px; */

            /* 
                border-radius 可以分别指定四个角的圆角
                    四个值 左上 右上 右下 左下
                    三个值 左上 右上/左下 右下 
                    两个个值 左上/右下 右上/左下  
              */
            /* border-radius: 20px / 40px; */

            /* 将元素设置为一个圆形 */
            border-radius: 50%;
        }
    </style>
</head>
<body>

    <!-- <div class="box1"></div> -->

    <div class="box2"></div>
</body>
</html>
```

**例**：-->[Here]()

## 字体

**例**：-->[Here]()

## 文本样式

**例**：-->[Here]()

## 背景

**例**：-->[Here]()

## 渐变

**例**：-->[Here]()

## 径向渐变

**例**：-->[Here]()

## 过渡

**例**：-->[Here]()

## 动画

**例**：-->[Here]()

## 变形

**例**：-->[Here]()

## z轴平移

**例**：-->[Here]()

## 旋转

**例**：-->[Here]()

## 缩放

**例**：-->[Here]()

# normal flow

网页是一个多层的结构，一层摞着一层，通过CSS可以分别为每一层来设置样式，作为用户来讲只能看到最顶上一层

这些层中，最底下的一层称为文档流，**文档流是网页的基础**

我们所创建的元素默认都是在文档流中进行排列

对于我们来元素主要有两个状态

## 在文档流中

![image-20220207141930469](C:\Users\LetengZzz\AppData\Roaming\Typora\typora-user-images\image-20220207141930469.png)

## 脱离文档流



**例**：-->[Here]()

# 附录

## 单位

```
 长度单位：
                    像素
                        - 屏幕（显示器）实际上是由一个一个的小点点构成的
                        - 不同屏幕的像素大小是不同的，像素越小的屏幕显示的效果越清晰
                        - 所以同样的200px在不同的设备下显示效果不一样

                    百分比
                        - 也可以将属性值设置为相对于其父元素属性的百分比
                        - 设置百分比可以使子元素跟随父元素的改变而改变

                    em
                        - em是相对于元素的字体大小来计算的
                        - 1em = 1font-size
                        - em会根据字体大小的改变而改变

                    rem
                        - rem是相对于根元素的字体大小来计算
```

## 颜色

```
 颜色单位：
                    在CSS中可以直接使用颜色名来设置各种颜色
                        比如：red、orange、yellow、blue、green ... ...
                        但是在css中直接使用颜色名是非常的不方便

                    RGB值：
                        - RGB通过三种颜色的不同浓度来调配出不同的颜色
                        - R red，G green ，B blue
                        - 每一种颜色的范围在 0 - 255 (0% - 100%) 之间
                        - 语法：RGB(红色,绿色,蓝色)

                    RGBA:
                        - 就是在rgb的基础上增加了一个a表示不透明度
                        - 需要四个值，前三个和rgb一样，第四个表示不透明度
                            1表示完全不透明   0表示完全透明  .5半透明

                    十六进制的RGB值：
                        - 语法：#红色绿色蓝色
                        - 颜色浓度通过 00-ff
                        - 如果颜色两位两位重复可以进行简写  
                            #aabbcc --> #abc
                    
                    HSL值 HSLA值
                        H 色相(0 - 360)
                        S 饱和度，颜色的浓度 0% - 100%
                        L 亮度，颜色的亮度 0% - 100%
```

## 网页的基本布局



## 项目
