---
title: 2017-9-27 
tags: 
author:sf
grammar_cjkRuby: true
---
## Course1
2017年09月27日 11时35分55秒
### 高级语言的优点
1. 高级语言接近于自然语言，独立于机器

	*  硬件独立性
	*  效率高
	*  可理解性，可移植性

2. 环境透明性

	* 不必考虑程序中的环境变量和常量的存储单元的分配问题
	* 不必考虑数据的外部形势钻换成机器的内部形式等细节
	* 不必了解程序运行环境是如何建立和维护的

### 翻译程序
 1. 编译:

	* 汇编程序:汇编语言->机器语言
	* 编译程序:高级语言->汇编 机器原因

 2. 解释:
	* 是一种模拟器,其机器语言是要被翻译的语言
	* 解释程序解释执行源程序但是不生成目标代码

 3. 高级语言的编译和执行阶段
 4. 解释程序同时处理源程序和数据
 5. 语句解释过程:
	 1. 解释程序先将源程序转换成一棵树
	 2. 遍历该树,执行节点上所规定的操作

### 编译的阶段
 1. 分析阶段:根据源语言的定义,分析源程序的结构
	* 词法分析
	* 语法分析
	* 语义分析 
 2. 综合阶段:根据分析结果构造出所要求的目标程序
	* 中间代码生成
	* 代码优化
	* 目标代码生成
 3. 符号表的管理
 4. 错误诊断和处理