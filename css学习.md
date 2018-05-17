
```
css背景属性:
background --> 简写属性,作用是将背景属性设置在一个声明中
background-attachment --> 背景图像是否固定或者随着页面的其余部分滚动
background-color --> 设置元素的背景颜色
background-image --> 把图像设置为背景
background-position --> 设置背景图像的起始位置
background-repeat --> 设置背景图像是否及如何重复
css文本格式:
color:blue --> 直接声明
color:#00ff00 --> 十六进制
color:rgb(255,0,0) --> rgb格式
w3c标准:如果你定义了颜色属性,还必须定义背景色属性
文本对齐方式:
text-align:center
text-align:right
text-align:justify --> 每一行展开宽度相等,左右外边距对齐
文本修饰:
text-decoration:overline --> 上面的划线
text-decoration:line-through --> 中间的划线
text-decoration:underline --> 下划线
文本转换:
text-transform:uppercase --> 大写
text-transform:lowercase --> 小写
text-transform:capitalize --> 首字母大写
文本缩进:
text-indent:50px
letter-spacing --> 指定字符之间的空间
line-height --> 行与行之间的空间
direction:rtl -->改变元素的文本方向 ltr(默认)
word-spacing --> 增加单词之间的空白空间
white-space:nowrap --> 禁用一个元素内的蚊子环绕(不换行)
vertical-align --> 垂直对齐图像
text-shadow:3px 6px #ddd --> 文本阴影

unicode-bidi: normal|embed|bidi-override|intitial|inherit; -->设置或返回文本是否被重写

css字体:
分通用字体系列和特定字体系列
Serif-->行的末端拥有额外的装饰
Sans-serif -->在末端没有额外的装饰
Monospace -->所有的等宽字符具有相同的宽度
font-family:"Times New Roman", Times, serif;-->多字体系列
字体样式:
font-style:normal --> 正常
font-style:italic --> 斜体
font-style:oblique --> 倾斜(不太支持)
字体大小:16px=1em(em的尺寸单位由W3C建议)
设置 <body>元素的默认字体大小的是百分比
body {font-size:100%;}
h1 {font-size:2.5em;}
font-weight --> 字体加粗
font-variant --> 字体的转变,以小型大写字体或者正常字体显示文本。
font:italic bold 12px/30px Georgia,serif --> 简写属性将字体属性设置在一个声明之内
链接样式:
a:link {color:#FF0000;} --> 未访问链接
a:visited {color:#00FF00;} --> 已访问链接
a:hover {color:#FF00FF;} --> 鼠标移动到链接上
a:active {color:#0000FF;} --> 鼠标点击时
#a:hover 必须跟在 a:link 和 a:visited后面
#a:active 必须跟在 a:hover后面
text-decoration --> 主要用于删除链接中的下划线(a:link {text-decoration:underline;})
a:link {background-color:#B2FF99;} --> 链接背景颜色
列表:
list-style-type --> 派指列表类型
list-style-image:url('sqpurple.gif') --> 作为列表项标记的图像

兼容性:
ul:设置列表样式类型为没有删除列表项标记:
ist-style-type:none
padding:0px
margin:0px
li: 无重复,定位,放置列表
background-repeat: no-repeat;
background-position: 0px 5px; 
padding-left: 14px;
列表 -缩写属性
list-style-type: circle
list-style-type: square
list-style-type: upper-roman
list-style-type: lower-alpha
list-style: square url("sqpurple.gif");
简写属性:list-style
顺序为:
list-style-type --> 列表项标志的类型
list-style-position --> 设置列表中列表项标志的位置
list-style-image --> 将图象设置为列表项标志
表格:
请注意，在上面的例子中的表格有双边框。这是因为表和th/ td元素有独立的边界。
为了显示一个表的单个边框，使用 border-collapse属性
border --> 边框
width-->宽度 height-->高度
表格文字对齐:
text-align
表格填充:
padding:上px 下px 左px 右px
表格颜色:(背景和颜色等)
background-color:green;
color:white;
定位表格标题:
caption {caption-side:bottom;}
盒子模型:
width(宽度)
Margin(外边距) - 清除边框外的区域，外边距是透明的。
Border(边框) - 围绕在内边距和内容外的边框。
Padding(内边距) - 清除内容周围的区域，内边距是透明的。
Content(内容) - 盒子的内容，显示文本和图像。

浏览器兼容性:
不要给元素添加具有指定宽度的内边距，而是尝试将内边距或外边距添加到元素的父元素和子元素。
IE8 及更早IE版本不支持 填充的宽度和边框的宽度属性设置。

解决IE8及更早版本不兼容问题可以在HTML页面声明 <!DOCTYPE html>即可。

边框样式:
border-style:none 无边框
border-style:dotted 虚线边框
border-style:dashed 虚线边框
border-style:solid 实线边框
border-style:double 双边框
border-style:groove 凹槽边框
border-style:ridge 垄断边框
border-style:inset 嵌入边框
border-style:outset 外凹边框
border-style:hidden 隐藏边框
border-width --> 属性为边框指定宽度。
3 个关键字之一，它们分别是 thick 、medium（默认值） 和 thin。
注意：CSS 没有定义 3 个关键字的具体宽度，所以一个用户可能把 thick 、medium 和 thin 分别设置为等于 5px、3px 和 2px，而另一个用户则分别设置为 3px、2px 和 1px。
"border-width" 属性 如果单独使用则不起作用。要先使用 "border-style" 属性来设置边框。
border-color单独使用是不起作用的，必须得先使用border-style来设置边框样式。
实例
可以指定不同的侧面不同的边框:
border-top-style:dotted;
border-right-style:solid;
border-bottom-style:dotted;
border-left-style:solid;
border-style属性可以有1-4个值(上下左右)
四边的颜色设置:
border-color:#ff0000 #00ff00 #0000ff rgb(250,0,255);
你可以在"border"属性中设置：
border-width
border-style (required)
border-color
上下左右都有三种属性:
下:
border-bottom
border-bottom-color
border-bottom-style 
border-bottom-width 

css轮廓:
outline
outline-style
outline-color
outline-width
外边距:可以使用cm(厘米)和%(百分比)
margin
margin-top
margin-bottom
margin-right
margin-left
填充:
padding
padding-top
padding-bottom
padding-right
padding-left
分组选择器(逗号分隔)
嵌套选择器(空格)
尺寸(Dimension)
控制元素的高度和宽度。同样，它允许你增加行间距
max-height --> 最大高度
max-width --> 最大宽度
min-heigh --> 最小高度
min-width --> 最小宽度
css显示和可见性
display属性设置一个元素应如何显示，visibility属性指定一个元素应可见还是隐藏。
visibility:hidden可以隐藏某个元素，但隐藏的元素仍需占用与未隐藏之前一样的空间。也就是说，该元素虽然被隐藏了，但仍然会影响布局。
display:none可以隐藏某个元素，且隐藏的元素不会占用任何空间。也就是说，该元素不但被隐藏了，而且该元素原本占用的空间也会从页面布局中消失。
块元素和内联元素:
display: inline --> 设置为内联元素
display:block --> 设置为块元素
border-collapse 属性设置表格的边框是否被合并为一个单一的边框
css定位:
static定位,没有定位,不受到上下左右影响
fixed定位,相对于浏览器窗口是固定位置
Relative 定位,相对其正常位置
即使相对定位元素的内容是移动,预留空间的元素仍保存在正常流动.
相对定位元素经常被用来作为绝对定位元素的容器块
absolute定位
绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于<html>
z-index
注意:如果两个定位元素重叠，没有指定z - index，最后定位在HTML代码中的元素将被显示在最前面
clip --> 剪辑一个绝对定位的元素
cursor --> 显示光标移动到指定的类型
overflow --> 设置当元素的内容溢出其区域时发生的事情
overflow-Y --> 顶部/底部边缘内容溢出时的处理
overflow-X --> 左边/右边边缘内容溢出时的处理
css浮动:会使元素向左或向右移动，其周围的元素也会重新排列
float:left/right --> 左右浮动
clear:both --> 清除浮动
line-height --> 行高
css水平对齐:
margin:auto;
如果宽度是100%,对齐没有效果.
ie5兼容性:增加外层div元素包裹,text-align:center,内层:margin-left:auto;margin-right:auto;text-align:left;width:70%;
使用position属性设置左右对齐
预先确定margin和元素的填充，始终是一个好主意:
body{margin:0;padding:0}
使用float属性设置左右对齐
css组合选择器:
后代选择器:空格
子元素选择器:大于号(只是当前的子)
相邻兄弟选择器:+号(下一个)
普通兄弟选择器:~(不在当前元素中的所有元素)
css伪类:
p > i:first-child
{
color:blue;
} 
<p>I am a <i>strong</i> man. I am a <i>strong</i> man.</p>
css lang伪类:q元素
q:lang(no)
{
quotes: "~" "~";
}
<p>Some text <q lang="no">A quote in a paragraph</q> Some text.</p>
input:focus
{
background-color:yellow;
}

所有的伪类元素:
:checked;选择没有选中的元素
:disable;选择所有禁用的表单元素
:empty;选择没有子元素的元素
:enabled;选择所有启用的表单元素
:first-of-type;选择每个父元素是某个元素的第一个元素
:in-range;选择元素指定范围的值
:invalid;选择所有无效的元素
:last-child;选择所有某元素的最后一个子元素
:last-of-type;选择没有某元素是其母元素的最后一个元素
:not(selector);除了某元素之外的所有元素
:nth-child(n);选择所有某元素的第二个子元素
:nth-last-child(n);选择所有某元素倒数的第二个子元素
:nth-last-of-type(n);选择所有某元素倒数的第二个为某元素的子元素
:nth-of-type(n);选择所有某元素第二个为p的子元素
:only-of-type;选择所有仅有一个子元素为某元素
:only-child;选择所有仅有一个子元素的某元素
:optional;选择没有"required"的元素属性
:out-of-range;选择指定范围以外的值的元素属性
:read-only;选择只读属性的元素
:read-write;选择没有只读属性的元素
:required;选择有required属性指定的元素属性
:root;选择文档的根元素
:target;选择当前活动的元素
:valid;选择所有有效值的属性
:link;选择所有未访问链接
:visited;选择所有访问过的链接
:active;选择正在活动链接
:hover;把鼠标放在链接上的状态
:focus;选择元素输入后具有焦点
:first-letter;选择每个某元素的第一个字母
:first-line;选择每个<p> 元素的第一行
:first-child;选择器匹配属于任意元素的第一个子元素的某元素
:before;在每个某元素之前插入内容
:after;在每个某元素之后插入内容
:lang(language);为某元素的lang属性选择一个开始值
伪元素:伪元素只能用于块级元素。
:first-line 选择每个某元素的第一行
:first-letter 选择每个某元素的第一个字母
```
