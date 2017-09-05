# 块级元素和行内元素分别有哪些？动手测试并列出4条以上的特性区别
```
块级元素：div h1 h2 h3 h4 h5 h6 p hr form ul dl ol pre table li dd dt tr td th 
行内元素：em strong span a br img button input label select textare code script
二者区别：
a.块级可以包括块级和行内；行内只能包含文本和行为
b.块级占据一整行空间；行内占据自身宽度空间
c块级可以进行宽高的设置；行内不可以设置宽高
d.块级可以进行内外边距的设置；行内对左右内外边距生效，对上下内外边距“在加边框和背景色时可以看到效果，但实际上本身高度没有变化”。
```
# 什么是 CSS 继承? 哪些属性能继承，哪些不能？
```
CSS继承就是子元素继承了父元素的CSS样式的属性
不可继承的：display、margin、border、padding、background、height、min-height、max-height、width、min-width、max-width、overflow、position、left、right、top、bottom、z-index、float、clear、table-layout、vertical-align、page-break-after、page-bread-before和unicode-bidi。
所有元素可继承：visibility和cursor。
内联元素可继承：letter-spacing、word-spacing、white-space、line-height、color、font、font-family、font-size、font-style、font-variant、font-weight、text-decoration、text-transform、direction。
终端块状元素可继承：text-indent和text-align。
列表元素可继承：list-style、list-style-type、list-style-position、list-style-image。
```
# 如何让块级元素水平居中？如何让行内元素水平居中?
```
块级元素水平居中：margin:0，auto
行内元素水平居中：text-align: center
```
# 用 CSS 实现一个三角形
```
#triangle{
width:0;
height:0;
border-left:20px solid transparent;
border-right:20px solid transparent;
border-bottom:20px solid blue;
}
```
5. 单行文本溢出加...如何实现?
```
white-space:nowrap;
overflow:hidden;
text-overflow:ellipsis;
 ```
6. px, em, rem 有什么区别
```
px:固定单位。
em: 相对单位，相对父元素字体的大小。（倍数）
rem:相对单位，相对于跟元素（html）字体的大小。（倍数）
```
7. 解释下面代码的作用?为什么要加引号? 字体里\5b8b\4f53代表什么?
```
body{font:12px/1.5tahoma,arial,'Hiragino Sans GB','\5b8b\4f53',sans-serif;}
表示字体规格为：
字体大小为12px
字体行高为1.5倍字体大小
字体可在tahoma,arial,'Hiragino Sans GB','\5b8b\4f53',sans-serif 这些字体中选择（若都不存在，则为浏览器默认字体）
当有空格或者Unicode码时，需要加引号
\5b8b\4f53是字体的Unicode码，表示黑体
```
