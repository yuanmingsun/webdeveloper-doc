##### 网页由三部分组成
- 结构
- 表现
- 行为
##### 对应的标准也分为三个部分
- 结构化标准语言包括xhtml和xml
- 表现标准语言包括了css
- 行为标准语言包括了e'cmascript


---
- HTML指超文本标记语言
- XHTML指可扩展的超文本标记语言
- HTML5指的html第五次改版

---
##### html5的基本结构

```
<!DOCTYPE html>命名文档类型

<html></html>说明我们写的是标记语言

<head></head>文件头部

<title></title>文件标题（显示在状态栏上的内容）

<meta charset=”utf-8”>编码格式

<body></body>文件主体（所有要写的内容）
```

```
<u></u>下划线标记，用来为文本加下划线

<br />空标记，用来设置字体换行

<hr />空标记，水平线

<span></span>文本结点，可以是某一小段文本，或是某一个字。
```
##### html三种列表
1. 无序列表

```
<ul>

<li>列表项内容</li>

<li>列表项内容</li>

<li>列表项内容</li>

</ul>
```
2. 有序列表
```
<ol>

<li>列表项内容</li>

<li>列表项内容</li>

<li>列表项内容</li>

</ol>
```

3.自定义列表


```
<dl>

<dt>名词</dt>

<dd>解释</dd>

</dl>
```

##### 超链接


```
<a href=”#”></a>空连接。

<a href=”目标文件路径及全称/连接地址(http://www. baidu.com)” alt=”替换文本” title=”提示文本”>链接文本/图片</a>

alt是当链接不对或者图片错误无法显示时出现的提示。

titile是鼠标移动上去之后显示的内容。

链接到email：

<a href=”mailto:1525676@163.com”>邮箱</a>

下载链接：

<a href=”aa.zip”>文件下载</a>

```

##### 图像

  地址相对路径的写法：

1. 当当前文件与目标文件在同一目录下，直接书写目标文件文件名+扩展名；

2. 当当前文件与目标文件所处的文件夹在同一目录下，写法如下：

文件夹名/目标文件全称+扩展名；

3. 当当前文件所处的文件夹和目标文件所处的文件夹在同一目录下，写法如下：

../目标文件所处文件夹名/目标文件文件名+扩展名；
```
<img src=”目标文件路径及全称” alt=”图片替换文本” title=”图片标题”/>
```


###### 表格


```
<table>

<tr>

   <td></td>

</tr>

</table>

注意：一对tr表示一行；一对td表示一列（一个单元格）

数据表格的相关属性：

1.width=”表格的宽度”

2.height=”表格的高度”

3.border=”表格的边框”

4.bordercolor=”边框色”

5.cellspacing=”单元格与单元格之间的间距”

6.cellpadding=”单元格与内容之间的空隙”

7.align=”表格对齐方式” 取值：left, right, center,

  valign=”垂直对齐”top/middle/bottom

8.合并单元格属性：

合并列：colspan=”所要合并的单元格的列数”

合并行：rowspan=”所要合并的单元格的行数”
```

##### 表单


```
1、表单框

<form name=”表单名称” method=”post/get” action=””></form>

说明：Get是用来从服务器上获得数据，而Post是用来向服务器上传递数据。处于安全性考虑，建议最好使用Post提交数据

2、表单控件

<input type=””/>

 

1,文本框

<imput type=”text” value=”默认值”/>

2.密码框

<input type=”password”/>

3.提交按钮

<input type=”submit” value=”按钮内容”/>

4.重置按钮

<input type=”reset” value=”按钮内容”/>

5.单选框/单选按钮

<input type=”radio” name=”ral”/>

<input type=”radio” name=”ral” checked=”checked”/>(默认选中）单选按钮中必须要写name，并且同一组单选中name要一样才能保证单选。

6.复选框

<input type=”checkbox” name=”like”/>

<input type=”checkbox” name=”like” disabled=”disabled”/>

(disabled=”disabled”:禁用；checked=”checked”:默认选中；html5中直接写disable和checked效果一样）

7.按钮

<input name=”” type=”button” value=”按钮内容”/>

（他和submit的区别是，submit是提交按钮，起到提交信息的作用，button只起到跳转的作用，不进行提交。）

 

下拉菜单：表示下拉列表，用户从这个列表中可以选择一个或多个选项。name属性不是必须的。

<select name=””>

<option>下拉选项</option>

......

</select>

 

多行文本框（文本域）：多行文本。rows属性和cols属性用来设置文本输入窗口的高度和宽度，单位是字符。

<textarea name=”” cols=”” rows=””></textarea>
```



