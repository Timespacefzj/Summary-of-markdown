&emsp;&emsp;最近刚上手CSDN的Markdown，发现其在编辑公式和排版方面确实相当好用， 还支持LaTex语法，CSS样式等，功能相当强大。经过一天的探索和学习，在这里好好总结一下涉及的相关知识点，以备自己查看和后来者学习。

[TOC]

#一、常用语法总结
（以下内容以便日后写作时直接复制，23333~）
>段首空格：`&emsp;&emsp; `
>&emsp;&emsp;<font color=red >**如果直接敲空格或TAB键会进入代码区，导致许多语法不能正常使用！**</font>
>标题级别：# 
>&emsp;&emsp;<font color=red >**使用几级标题就写几个#**</font>
>无序列表：*+（空格）
>有序列表：（数字）+.+（空格）

>斜体字符：\*……*
>粗体字符：\**……**
>删除文字：~~&emsp;&emsp; ~~

>表格：|--------|---------|--------|
>表格左对齐：|：--------|
>表格中对齐：|----：----|
>表格右对齐：|--------：|
>换行：\\ 
>段落缩进：- 半方大的空白`&ensp;或&#8194; `,全方大的空白`&emsp;或&#8195; `，不断行的空白格`&nbsp;或&#160; ` 。

>代码块：缩进每一行由至少 4 个空格或 1 个制表符Tab。
>代码块高亮：三个反撇+（代码语言名）
>&emsp;&emsp;<font color=red >1.在需要高亮的代码块的前一行及后一行使用三个反引号，同时第一行反引号后面表面代码块所使用的语言。
>&emsp;&emsp;2.在代码块中插入代码块的Markdown格式时，需要在反引号之前添加空格，否则呈现的布局会超出你的预期。</font>

>行内公式：\$…\$
>块公式：\$\$…\$\$
>引用：>
>内联代码字符：\`……`
>超链接：[连接名]+（链接地址url）
>插入图片：！[图片名称]+（图片地址）
>"&"符号：& amp; 
>横线分隔符：- - -（段前段后各空一行）
>插入自动目录：[TOC]

----

#二、字体调整

##1.字体
{\rm text}如： 
使用罗马字体：${\rm text}$ ，`${\rm text}$`

**其他的字体还有：** 
代码|字体|代码|字体
:-|:-|:-|:-
\rm|${\rm 罗马体}$|\it|${\it 意大利体}$ 
\bf|${\bf 黑体}$|\cal|${\cal 花体}$ 
\Bbb|${\Bbb 黑板粗体字}$|sf|${\sf 等线体}$ 
\mit|${\mit 数学斜体}$|\tt|${\tt 打字机字体}$ 
\scr|${\scr 小体大写字母}$|


----

##2.字体颜色
格式：`$\color{颜色}{语句}$`

例如：
>\$\color{green}{Hello World!}$\
>$\color{green}{Hello World!}$

代码|效果	
:-| :-
`$\color{black}{Hello World!}$`|$\color{black}{Hello World!}$	
`$\color{gray}{Hello World!}$`|$\color{gray}{Hello World!}$
`$\color{silver}{Hello World!}$`|$\color{silver}{Hello World!}$
`$\color{white}{Hello World!}$`|$\color{white}{Hello World!}$
`$\color{maroon}{Hello World!}$`|$\color{maroon}{Hello World!}$
`$\color{red}{Hello World!}$`|$\color{red}{Hello World!}$
`$\color{yellow}{Hello World!}$`|$\color{yellow}{Hello World!}$
`$\color{lime}{Hello World!}$`|	$\color{lime}{Hello World!}$
`$\color{olive}{Hello World!}$`|$\color{olive}{Hello World!}$
`$\color{green}{Hello World!}$`|$\color{green}{Hello World!}$
`$\color{teal}{Hello World!}$`|	$\color{teal}{Hello World!}$
`$\color{aqua}{Hello World!}$`|$\color{aqua}{Hello World!}$
`$\color{blue}{Hello World!}$`|$\color{blue}{Hello World!}$
`$\color{navy}{Hello World!}$`|$\color{navy}{Hello World!}$
`$\color{purple}{Hello World!}$`|$\color{purple}{Hello World!}$	
`$\color{fuchsia}{Hello World!}$`|	$\color{fuchsia}{Hello World!}$


---

##3.内嵌HTML

使用HTML代码可调整字体、字号、字体颜色、背景色。

>`<font face="宋体">我是宋体字</font>`
>`<font face="微软雅黑">我是微软雅黑</font>`
>`<font face="STCAIYUN">我是华文彩云</font>`
`<font color=red >color=red</font>`
`<font color=#0099ff size=3>color=#0099ff </font>`
`<font color=#00ffff size=5>color=#00ffff</font>`
`<table><tr><td bgcolor=#7FFFD4>背景色是天蓝色</td></tr></table>`

<font face="宋体">我是宋体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=red >color=red</font>
<font color=#0099ff size=3>color=#0099ff </font>
<font color=#00ffff size=5>color=#00ffff</font>

<table><tr><td bgcolor=#7FFFD4>背景色是天蓝色</td></tr></table>

<font color=red size=3>**注：字号可能的值为从 1 到 7 的数字，浏览器默认值是 3。**
</font>



---



#三、表格

##1.实现方式

两种最为直观的创建表格方式：

-  简单方式

>姓名 | 学科 | 分数
	- | :-: | -: 
小明| 数学| 90 
小红 | 物理 | 85
小张| 化学 | 80

姓名 | 学科 | 分数
- | :-: | -: 
小明| 数学| 90 
小红 | 物理 | 85
小张| 化学 | 80


---
- 原生方式
>|姓名 | 学科 | 分数|
	|- | :-: | -:| 
|小明| 数学| 90 |
|小红 | 物理 | 85|
|小张| 化学 | 80|

--
|姓名 | 学科 | 分数|
|- | :-: | -:| 
|小明| 数学| 90 |
|小红 | 物理 | 85|
|小张| 化学 | 80|


---

##2.语法说明：

1. 不管是哪种方式，第一行为表头，第二行分隔表头和主体部分，第三行开始每一行代表一个表格行； 
2. 列与列之间用管道符号 “|” 隔开，原生方式的表格每一行的两边也要有管道符。 
3. 可在第二行指定不同列单元格内容的对齐方式，默认为左对齐，在 “-” 右边加上 “:” 为右对齐，在 “-” 两侧同时加上 “:” 为居中对齐。

---

##3.参数调整：

>| 参数 |备注| 
	| - | - | 
| -l |以长列表方式显示（显示出文件/文件夹详细信息） | 
| -t |按照修改时间排序（默认最近被修改的文件/文件夹排在最前面） | 
|-r | 逆序排列|
| 参数 |备注| 
| - | - | 
| -l |以长列表方式显示（显示出文件/文件夹详细信息） | 
| -t |按照修改时间排序（默认最近被修改的文件/文件夹排在最前面） | 
|-r | 逆序排列|


---

##4.内嵌HTML
源代码为：

``` HTML
		<table>
		  <tr>
		    <th width=40%, bgcolor=yellow >参数</th>
		    <th width="60%", bgcolor=yellow>备注</th>
		  </tr>
		  <tr>
		    <td bgcolor=#eeeeee> -l </td>
		    <td> 以长列表方式显示（显示出文件/文件夹详细信息）  </td>
		  </tr>
		  <tr>
		    <td bgcolor=#00FF00>-t </td>
		    <td> 按照修改时间排序（默认最近被修改的文件/文件夹排在最前面） </td>
		  <tr>
		    <td bgcolor=rgb(0,10,0)>-r </td>
		    <td>  逆序排列 </td>
		  </tr>
		</table>
```


<table>
		  <tr> 
		    <th width=20%, bgcolor=yellow >参数</th>
		    <th width="80%", bgcolor=yellow>备注</th>
		  </tr>
		  <tr>
		    <td bgcolor=#eeeeee> -l </td>
		    <td> 以长列表方式显示（显示出文件/文件夹详细信息）  </td>
		  </tr>
		  <tr>
		    <td bgcolor=#00FF00>-t </td>
		    <td> 按照修改时间排序（默认最近被修改的文件/文件夹排在最前面） </td>
		  <tr>
		    <td bgcolor=rgb(0,10,0)>-r </td>
		    <td>  逆序排列 </td>
		  </tr>
</table>



---

---

#四、流程图

##1.UML时序图
&emsp;&emsp;时序图，亦称为序列图或循序图，是一种UML行为图。它通过描述对象之间发送消息的时间顺序显示多个对象之间的动态协作。它可以表示用例的行为顺序，当执行一个用例行为时，时序图中的每条消息对应了一个类操作或状态机中引起转换的触发事件。

---

###时序图元素
时序图中包括5种元素：角色，对象，生命线，激活期和消息.。

- **角色（Actor）**

>系统角色，可以是人或者其他系统，子系统。

- **对象(Object)**

>对象代表时序图中的对象在交互中所扮演的角色，位于时序图顶部和对象代表类角色。 
对象一般包含以下三种命名方式： 
第一种方式包含包含对象名和类名 
第二种方式只显示类名不显示对象名，即为一个匿名对象。 
第三种方式只显示对象名不显示类名。

- **生命线(Lifeline)**

>生命线代表时序图中的对象在一段时期内的存在。时序图中每个对象和底部中心都有一条垂直的虚线，这就是对象的生命线，对象间 的消息存在于两条虚线间。

- **激活期(Activation)**

>激活期代表时序图中的对象执行一项操作的时期，在时序图中每条生命线上的窄的矩形代表活动期。它可以被理解成C语言语义中一对花括号“{}”中的内容

- **消息(Message)**

>消息是定义交互和协作中交换信息的类，用于对实体间的通信内容建模，信息用于在实体间传递信息。允许实体请求其他的服务，类角色通过发送和接受信息进行通信。

###时序图建立方法

**说明：**->中，-代表实线，>代表实心箭头，还可以用--表示虚线，>>表示非实心箭头。在UML时序图中，实线表示主动发送消息，虚线表示返回（应答）消息，实心箭头表示同步消息（消息发送者停止活动等待应答消息），非实心箭头表示异步消息（消息发送者无须停止活动等待应答消息）。->两边可以是同一个Actor，表示自交互。

**示例：**
>\` \` \` sequence
客户端->打印机: 打印请求(id)
打印机->数据库:请求数据(id)
Note right of 数据库: 执行SQL获取数据
数据库-->打印机:返回数据信息
Note right of 打印机:使用数据打印
打印机-->>客户端:返回打印结果
客户端->客户端:等待提取结果
\` \` \` 

``` sequence
客户端->打印机: 打印请求(id)
打印机->数据库:请求数据(id)
Note right of 数据库: 执行SQL获取数据
数据库-->打印机:返回数据信息
Note right of 打印机:使用数据打印
打印机-->>客户端:返回打印结果
客户端->客户端:等待提取结果
```
---
##2.UML流程图

流程图的语法大体分为两部分：

- 前面部分用来定义流程图元素；
- 后面部分用来连接流程图元素，指定流程图的执行走向。

###定义元素阶段语法：
>tag=>type: content:>url

说明：

>- tag 是流程图中的标签，在第二段连接元素时会用到。名称可以任意，一般为流程的英文缩写和数字的组合。
- type 用来确定标签的类型，`=>`后面表示类型。由于标签的名称可以任意指定，所以要依赖type来确定标签的类型
标签有6种类型：`start` `end` `operation` `subroutine` `condition` `input` `output`
- content 是流程图文本框中的描述内容，`:` 后面表示内容，中英文均可。特别注意，冒号与文本之间一定要有个`空格`
- url是一个连接，与框框中的文本相绑定，`:>`后面就是对应的 url 链接，点击文本时可以通过链接跳转到 url 指定页面

---

**常用语法：**

开始

	st=>start: 开始
操作

	op1=>operation: 操作、执行说明
条件

	cond=>condition: 确认？
结束

	e=>end: 结束
URL

	e=>点击本结束跳转:>http://网址

---
###连接流程图元素:
连接流程图元素阶段的语法就简单多了，直接用->来连接两个元素:
>st->op1->cond

几点说明如下：
>- 使用 -> 来连接两个元素
- 对于condition类型，有yes和no两个分支
- 每个元素可以制定分支走向，默认向下，也可以用right指向右边，如示例中sub1(right)。

**示例：**
源代码为：
>\` \` \` flow
st=>start: Start
e=>end: End
op1=>operation: My Operation
sub1=>subroutine: My Subroutine
cond=>condition: Yes or No?
io=>inputoutput: catch something...
st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
\` \` \` 

```flow
st=>start: Start
e=>end: End
op1=>operation: My Operation
sub1=>subroutine: My Subroutine
cond=>condition: Yes or No?
io=>inputoutput: catch something...
st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
```

---
#五、LeTex及数学公式
##1.简单的规则：
>1. 空格：LaTeX中空格用来隔开单词(英语一类字母文字)，多个空格等效于一个空格；对中文没有作用。 
2. 换行：用控制命令“\”,或“ \newline”. 
3. 分段：用控制命令“\par” 或空出一行。 
4. 换页：用控制命令“\newpage”或“\clearpage” 
5. 特殊控制字符：#，$, %, &, - ,{, }, ^, ~ 
6. 上、下划线：\overline｛…｝和\underline｛…｝
7. 上、下水平大括号：\overbrace｛…｝\_｛…｝和\underbrace｛…｝\_｛…｝
8. 省略号：\ldots 表示语文本底线对其的省略号，\cdots表示与文本中线对其的省略号。
##2.希腊字母
![这里写图片描述](http://img.blog.csdn.net/20171005214132219?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

如果使用大写的希腊字母，把命令的首字母变成大写即可，例如 \Gamma 输出的是$\Gamma$。

如果使用斜体大写希腊字母，再在大写希腊字母的LaTeX命令前加上var，例如\varGamma 生成 $\varGamma$。
##3.分数和矢量

**分数线：**\frac｛分子｝｛分母｝，或者 分子\over 分母
例如：$\frac{x}{x+1}$，或者$x\over{x+1}$
**矢量：**\vec{…}
示例：$\vec{a} \cdot \vec{b}=0$

##4.和号和积分号
![这里写图片描述](http://img.blog.csdn.net/20171005214232889?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##5.其它常用命令
![这里写图片描述](http://img.blog.csdn.net/20171005214254575?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##6.特殊公式格式
- **分数导致字母太小**

在LaTeX中若用`\frac`有时会导致字母显示出来很小，解决方案是使用`\dfrac`。其中\dfrac即为\displaystyle\frac的意思。例如：
>x=\dfrac{a_{22}b_1-a_{21}b_2}{a_{11}b_{2}-a_{12}b_{1}}

$$x=\dfrac{a_{22}b_1-a_{21}b_2}{a_{11}b_{2}-a_{12}b_{1}}$$

- **多行方程组对齐**

>\ begin{cases} 
&emsp;&emsp;a_{11}x_1&+&a_{12}x_2&+&\cdots&+a_{1n}x_n&=&b_1\\
&emsp;&emsp;&&&&\vdots\\
&emsp;&emsp;a_{n1}x_1&+&a_{n2}x_2&+&\cdots&+a_{nn}x_n&=&b_n&			
\ end{cases}
	
$$\begin{cases} 
		a_{11}x_1&+&a_{12}x_2&+&\cdots&+a_{1n}x_n&=&b_1\\
		&&&&\vdots\\
		a_{n1}x_1&+&a_{n2}x_2&+&\cdots&+a_{nn}x_n&=&b_n&			
	\end{cases}$$
	

- **多行公式等号对齐**

>\ begin{eqnarray}
f(x,y)
		&=&(x+y)^2-(x-y)^2\\
		&=&4xy
	\ end{eqnarray}

$$\begin{eqnarray}
f(x,y)&=&(x+y)^2-(x-y)^2\\
		&=&4xy
	\end{eqnarray}$$

- **大括号右多行赋值**

方法1：用 cases
>P(x|a_x)=
>\ begin{cases} 
1, & x=f(a_{x})\\ 
0, & other\ values 
\ end{cases}

方法2：用 array
>P(x|a_x)=
\ left\{\begin{array}{cc} 
1, & x=f(a_{x})\\ 
0, & other\ values 
\ end{array}\right.

<font color=red >**注：& 可以用来对齐。**</font>

$$P(x|a_x)=
\left\{\begin{array}{cc} 
1, & x=f(a_{x})\\ 
0, & other\ values 
\end{array}\right.$$

- **矩阵**

>\ left(\begin{array}{cc}
		1 & 2 \\ 
		3 & 4 
	\ end{array}\right)
	
$$\left(\begin{array}{cc}
		1 & 2 \\ 
		3 & 4 
	\end{array}\right)$$

- **求和符号上下限位置**

1. 默认情况下： 
a）默认行内公式`$\sum_{i=1}^n{x_i}$`的上下限标注在右侧：$\sum_{i=1}^n{x_i}$
b）默认行间公式`$$\sum_{i=1}^n{x_i}$$`上下限标注在上下：$$\sum_{i=1}^n{x_i}$$
2. 可强制修改：
a）强制行内公式`$\sum\limits_{i=1}^n{x_i}$`的上下限标注在上下：$\sum\limits_{i=1}^n{x_i}$
b）强制行间公式`$$\sum\nolimits_{i=1}^n{x_i}$$`上下限标注在右侧：$$\sum\nolimits_{i=1}^n{x_i}$$

- **求和符号下多行限制条件**

>\prod_{i_0,i_1,\ldots,i_m>0\atop 
		 i_0+i_1+\cdots,i_m=n}
		{A_{i_0}A_{i_1}\cdots A_{i_m}}
		
$$\prod_{i_0,i_1,\ldots,i_m>0\atop 
		 i_0+i_1+\cdots,i_m=n}
		{A_{i_0}A_{i_1}\cdots A_{i_m}}$$ 
		
- **条件偏导**

>\$\$\left.\frac{\partial f(x,y)}{\partial x}\right.|_{x=1}$$

$$\left.\frac{\partial f(x,y)}{\partial x}\right|_{x=1}$$
注：\left和\right必须成对出现，对于不显示的一边可以使用 . 代替

- **加大括号**

有时候括号需要大号的，普通括号不好看，此时需要使用\left和\right加大括号的大小
>\$(\frac{x}{y})^2$，$\left(\frac{x}{y}\right)^2\$

$$(\frac{x}{y})^2,\left(\frac{x}{y}\right)^2$$



---


#六、其他
##1.反斜杠转义符
&emsp;&emsp;Markdown 可以利用反斜杠来插入一些在语法中有其它意义的符号，例如：如果你想要用星号加在文字旁边的方式来做出强调效果（但不用 $<em>$ 标签），你可以在星号的前面加上反斜杠：\\* 字符星号 \\*

&emsp;&emsp;Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：
>\   反斜线
`   反引号
*   星号
_   底线
{}  花括号
[]  方括号
()  括弧
\#   井字号
+   加号
-   减号
.   英文句点
!   惊叹号

-----

##2.页内跳转
先定义一个标识（即以下这行代码），并把它放到要跳转的地方。 
<div id="footer"></div>
然后把跳转链接放在随意地方，当点击这个跳转链接的时候变回跳到当前标识所在的位置。 
[跳转到数学公式](#footer) 
比如我把标识代码放在数学公式的上一行，当点击跳转到数学公式的时候便会实现跳转。

---

##3.图片大小和对齐方式

使用HTML标记语言调整

- **图片大小：**

*值为正数*
`<img src="图片地址" width="宽度值" height="高度值" />`

- **图片对齐方式：**

*对齐方式包括：center，left，right*
>`<div align=对齐方式>
![图片描述](图片地址)
</div>`

---

#附录：LeTex符号表
##希腊字母
![这里写图片描述](http://img.blog.csdn.net/20171005205934348?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##二进制运算符
![这里写图片描述](http://img.blog.csdn.net/20171005210334516?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##关系符号
![这里写图片描述](http://img.blog.csdn.net/20171005210426811?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##数学运算符
![这里写图片描述](http://img.blog.csdn.net/20171005210715338?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##数学形式符号
![这里写图片描述](http://img.blog.csdn.net/20171005211953860?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##数学函数
![这里写图片描述](http://img.blog.csdn.net/20171005211448944?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##标点符号
![这里写图片描述](http://img.blog.csdn.net/20171005210506571?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##箭头符号
![这里写图片描述](http://img.blog.csdn.net/20171005210520244?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##分隔符
![这里写图片描述](http://img.blog.csdn.net/20171005211536370?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##大分隔符
![这里写图片描述](http://img.blog.csdn.net/20171005211743694?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##杂项符号
![这里写图片描述](http://img.blog.csdn.net/20171005210632121?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
##发音
![这里写图片描述](http://img.blog.csdn.net/20171005211900673?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2J3ZW0=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)






