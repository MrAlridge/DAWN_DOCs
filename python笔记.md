# 这个是用来补充说明的笔记本
==========================
## python对多行语句的分段
Python 通常是一行写完一条语句，但如果语句很长，我们可以使用反斜杠(\)来实现多行语句，例如：
```python
total = item_one + \
        item_two + \
        item_three
```
实际上就是:
```python
total = item_one + item_two + item_three
```
在 [], {}, 或 () 中的多行语句，不需要使用反斜杠(\)，例如：
```python
total = ['item_one', 'item_two', 'item_three',
        'item_four', 'item_five']
```
==========================
## python的基本类型(我觉得不用记)
python中数字有四种类型：整数(int)、布尔型(bool)、浮点数(float)和复数(complex)。
## 字符串相关
1.多行字符串可以用'''或"""括起来以表示.

2.反斜杠可以用来转义，使用r可以让反斜杠不发生转义。。 如 r"this is a line with \n" 则\n会显示，并不是换行。

3.字符串可以用 + 连接,用 *  重复

4.Python中的字符串不能改变。    //python中没有字符这一类型

5.字符串的截取的语法格式如下：变量[头下标:尾下标:步长]

[详见文件pyString.py](D:\DOCS\PYTHON_DOCs\pyString.py)
===================
## 空行
函数之间或类的方法之间用空行分隔，表示一段新的代码的开始。类和函数入口之间也用一行空行分隔，以突出函数入口的开始。

空行与代码缩进不同，空行并不是Python语法的一部分。书写时不插入空行，Python解释器运行也不会出错。但是空行的作用在于分隔两段不同功能或含义的代码，便于日后代码的维护或重构
## 语句分隔
与C语言一样,同一行的语句之间可以用 ; 来分隔
`import sys; x = 'runoob'; sys.stdout.write(x + '\n')`
## 代码组
冒号":"是代码组开始的标志,用以判断之后的缩进是否为同一组,作用类似于C语言中的花括号{}
```python
if case1 :
    event1()
elif case2 :
    event2()
else :
    event3()
```
========================
## 导入语句(import 与 from import)

在 python 用 `import` 或者 `from...import` 来导入相应的模块。

将整个模块"somemodule"导入，格式为： `import somemodule`

从某个模块中导入某个函数,格式为： `from somemodule import somefunction`

从某个模块中导入多个函数,格式为： `from somemodule import firstfunc, secondfunc, thirdfunc`

将某个模块中的全部函数导入，格式为： `from somemodule import *`

## 为多个语句赋值

支持以下方式赋值:
```python
a = b = c = 1 # 实际上就是从后向前赋值

a,b,c = 1,'str',True
```

## 标准数据类型注意事项

常量(不可变)有:数字,字符串,元组

变量有:字典,列表,集合(set)

可以使用`del`语句删除对象的引用,如:
```python
del target1,target2 # 可以一直删下去
```

数值的除法中,`/`得到的是浮点数,`//`得到的是整数

=======================

## 列表(List)

列表是写在方括号 [] 之间、用逗号分隔开的元素列表。

列表中的元素是可以随便添加的 ~~(啥都能往里塞)~~

列表的截取这样实现:
`变量名[头下表:尾下标]`

![alt list的图片](https://www.runoob.com/wp-content/uploads/2014/08/list_slicing1_new1.png "一看就懂了吧")

与字符串一样,可以使用 `+` 进行连接,使用 `*` 进行重复

`List`类内置了诸如`append()`,`pop()`等方法~~所以说赶快更到["那个文档"](D:\DOCS\python函数笔记.md)里面啊!!~~