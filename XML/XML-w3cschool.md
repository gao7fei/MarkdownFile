---
title: 2017-10-25未命名文件 
tags: 新建,模板,小书匠
grammar_cjkRuby: true
Teacher info:
name:
email:
tel:
---


欢迎使用 **{小书匠}(xiaoshujiang)编辑器**，您可以通过==设置==里的修改模板来改变新建文章的内容。
# XML基础
## XML简介
1. xml是被设计用来传输和存储数据，html是被设计用来显示数据
2. ==XML（EXtensible Markup Language,可扩展标记语言）==：
	* 是一种**标记语言**，类似于HTML
	* 设计宗旨是用来传输数据，而不是显示数据
	* XML标签没有被预定义。您需要自行定义标签
	* XML被设计为具有自我描述性

3. XML与HTML的主要差异：
	* XML与HTML的设计目的不同
	* XML被设计用来传输和存储数据，其焦点是数据的内容
	* HTML被设计用来显示数据。其焦点是数据的外观
	* HTML旨在显示信息，xml旨在传输信息

4. XML本身不会做任何事情，也就是说XML是不作为的。XML仅仅是纯文本，任何有能力处理纯文本的程序都能够处理XML
5. XML允许用户自行定义标签。

## XML应用
1. XML把数据从HTML中分离出来：简化HTML在显示动态数据，当需要修改数据的时候的工作量
2. XML简化了数据共享：XML数据使用纯文本格式进行存储，因此提供了一种独立于软件和硬件的数据存储方法
3. XML简化了平台的变更：理由大致同上
4. XML用于创建新的Internet语言

## XML树结构
1. XML提供了一种树结构，它从“根部”开始，然后扩展到“枝叶”·
2. 一个XML文档实例：

	``` xml
	<?xml version="1.0" encoding="ISO-8859-1"?>
	<note>
	<to>George</to>
	<from>John</from>
	<heading>Reminder</heading>
	<body>Don't forget the meeting!</body>
	</note>
	```
	* 第一行：XML声明，定义了XML的版本和所使用的编码
	* 第二行：描述了文档的根元素
	* 下面的四行：描述了4个子元素
	* 最后一行：定义了根元素的结尾

3. XML文档形成一种树结构

	``` xml
	<root>
	  <child>
		<subchild>.....</subchild>
	  </child>
	</root>
	```
	* XML文档必须包含根元素。该元素是所有其他元素的父元素
	* 所有元素均可拥有子元素
	* 父、子及同胞等术语用于描述元素之间的关系。父元素拥有子元素，相同层级 的子元素称为同胞。所有元素均可拥有文本内容和属性。

![enter description here][1]


  [1]: http://www.w3school.com.cn/i/ct_nodetree1.gif
  
## XML语法规则
1. 所有的XML元素都必须有关闭标签。（HTML标签不必如此）
	> XML 声明没有关闭标签。这不是错误。声明不属于XML本身的组成部分。不需要关闭标签
2. XML标签对大小写敏感
3. XML必须正确的嵌套（HTML不必要，但解析的结果可能因此而变得不确定）
4. XML文档必须有根元素
5. XML的属性值必须加引号
6. 实体引用：XML中的一些字符拥有特殊的意义，直接使用这些字符将会发生错误，应该使用实体引用来替换掉这些特殊字符。
7. XML中的注释：与HTML的注释类似。
8. 在XML中空格会被保留，HTML会把多个连续的空格字符裁剪成一个，而XML文档中的空格不会被删节。
9. XML以LF存储换行：在 Windows 应用程序中，换行通常以一对字符来存储：回车符 (CR) 和换行符 (LF)。这对字符与打字机设置新行的动作有相似之处。在 Unix 应用程序中，新行以 LF 字符存储。而 Macintosh 应用程序使用 CR 来存储新行。