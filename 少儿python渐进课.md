# 少儿PYTHON渐进课  
- [一.数据类型与变量](#一数据类型与变量) 
- [二.与用户的互动(input与print)](#二与用户的互动input与print) 
- [三.字符串常用操作](#三字符串常用操作) 
- [四.数值类型与数学运算问题](#四数值类型与数学运算问题) 
- [五.流程控制语句之条件判断](#五流程控制语句之条件判断) 
- [六.流程控制语句之循环](#六流程控制语句之循环) 
- [七.数据类型之列表](#七数据类型之列表) 
- [八.使用python控制硬件](#八使用python控制硬件) 
- [九.数据类型之字典](#九数据类型之字典)
- [十.函数或方法](#十函数或方法)
- [十一.类与对象](#十一类与对象)
- [十二.模块](#十二模块)



# 一.数据类型与变量
### 1.在python中常用的内置数据类型有哪些
    > 记住python中最常用的6种类型: Number（数字）、String（字符串）、Tuple（元组）； 可变数据（3 个）：List（列表）、Dictionary（字典）、Set（集合）
### 2.以下是python关键字
这些关键字不是全面的，但是最常用的，在学习的过程中要记住并知道它们代表的意义：
|关键字|程序语义|传统语义
--|--|--
print |打印，输出    |打印
string| 字符串类型       | 细绳
int|    整数类型|
float|  浮点类型|漂流物, 浮舟, 漂浮, 浮萍    
for| 计数循环,也叫for循环   |对于
in|  在里面|在里面
while| 条件循环，也叫while循环  |虽然,尽管
break| 跳出          |打破;(使)破，裂，碎;休息;间歇
continue| 不往下执行，直接下一个 |继续
False| 假    |错误的
True| 真      |符合事实的
None| 对象不存在    |没有一个
if|  条件判断语句关键字  |如果
else| 条件语句关键字   |其他的
elif| 再判断条件语句关键字| 完整英语 else if 
and| 并且        |和
or| 或者    |或者
not| 不是（取反）      |不
list| 列表      |列表
dictionary| 字典    |字典
class| 类      |班;班级
self| 类的本身    |自己，其他语言的this
pass| 占位    |通过
def| 定义(函数)|
return| 返回   |回来
global| 全局变量    |全球的;全世界的;整体的;全面的;总括的
import| 导入(模块里的对象，函数) |进口;输入;引进;导入;移入
try|    异常处理    |尝试，试图
except| 捕获异常   |除了;只是,不包括
raise|  抛出 异常   |提升;举起;提起
input| 输入 |输入; 输入的信息
range| 范围; |一系列

### 3.对字符串处理常用到的方法单词
```py
    replace : 替换
    join    : 将列表连接成字符串，      传统语义: 提升;举起;提起
    format  ：格式化,在python中的简写f  传统语义: 格式
    find    : 查找位置下标             传统语义:发现；找到；
    count   : 统计某个字条出现的次数    传统语义:总数；数数
    encode  : 编码
    split   : 将字符分割成列表          传统语义:裂口；裂缝 
    startswith: 开始包含
    endswith: 结尾包含
```

### 4.定义一个数值类型的变量
比如定义三个变量，给赋值一个三角形的长，宽，高
### 5.定义一个字符串类型的变量
比如定义一个变量，给它赋值我的名字
### 6.变量名称的起名规则与良好习惯

- 变量名称可以由字母、数字、下画线随意组合，长度也可以随意，但不要以数字开头
- 变量名称区分大小写
- 变量名称支持中文，但不建议使用中文 

- 7.如果查看一个变量的类型，提示采用：type()


# 二.与用户的互动(input与print)

### 1.如何打印出一个字符串或数字

练习：定义一个变量 abc="abcdef", 然后打印输出abc

### 2.接受用户输入一个字符
练习1：定义一个变量 abc, 用这个变量接收用户输入字符串，并打印输出abc
### 3.接受用户输入一个数字
练习2：定义一个变量 abc, 用这个变量接收用户输入一个数字，并让这个数字乘以10后打印输出

### 4.变量值的互换
要求用户输入x与y两个值，接收到这两个值并分别赋值给x与y,然后将这个两个值互换输出
```py
    # 用户输入
    
    x = input('输入 x 值: ')
    y = input('输入 y 值: ')
    
    # 创建临时变量，并交换
    temp = x
    x = y
    y = temp
    
    print('交换后 x 的值为: {}'.format(x))
    print('交换后 y 的值为: {}'.format(y))
```


# 三.字符串常用操作

### 1.什么是字符串的下标，提示 :str[下标] 从左向右0→+，从右向左 
下标与叫索引,是标记元素位置的顺序号，注意，索引都是从0开始，而不是从1开始。

```
想知道为什么在程序中很多标记起始位置的数字都是0而不是1妈?，因为二进制计数是从0开始的，为了不浪费比特位，所以内在位置和列表索引采用了从0开始
```

### 2.给一个变量赋值字符串的值 ，并返回这个字符串的长度(len)
 练习：abc = "abcdefg" 求出abc这个变量的长度
### 3.给一个变量赋值字符串的值，并返回指定位置的字符
 练习：abc = "abcdefg" 通过下标取出e这个字符
### 4.给一个变量赋值字符串的值，并返回指定符的位置
 初步了解对象与属性，如果通过.符号引用对象里的属性与方法
 提示使用.find() find函数的使用：如果包含子字符串返回开始的索引值，否则返回-1。
 练习：abc = "abcdefg" 找出e这个字符的下标
### 5.给一个变量赋值字符串的值，并返回指位置范围的字符
 练习：abc = "abcdefg" 通过下标取出def这个字符
### 6.判断某个字符是否存在 提示，使用 in,比如 'a' in 'abc' 
 练习：abc = "abcdefg"，检查"de"是否存在于abc这个变量中
### 7.查询某个字符在一个字符串中出现的次数，提示使用 .count()方法
 练习：abc = "abcdefgarao" 统计出abc这个变量包含多少个a
### 8.替换掉字符串中某个字符，提示使用.replace()
 练习：abc = "abcdefgarao" 将abc这个变量中的a替换成"***"三个星号

### 9.将字符串转换成大小定

### 10.字符串的连接
采用+号学与f两种连接方式即可
```py
    name_1 = '你的名字是：'
    name_2 = '陈明明'
```
1)采用以上说的两种方式，连接name_1与name_2并打印出:我的名字是陈明明
2)采用以上说的两种方式，连接name_1与name_2并打印出:大家好，我的名字是陈明明
3)采用以上说的两种方式，连接name_1与name_2，将连接的结果赋值给变量name_3,最后打印出name_3
### 11.去掉字符里的空白处
 1.去掉前后空白 提示:使用方法 .strip()
 2.去掉左边空白 提示:使用方法 .lstrip()
 3.去掉右边空白 提示:使用方法 .rstrip()

# 四.数值类型与数学运算问题
认识python中常用的数值类型(number,int float,long)

### 1.数学中的加减乘除在python中分别用什么符号表示
- 加法`+` 
- 减法`-`
- 乘法`*`
- 除法`/`
 
``` 
注：在python中任意两个数(那么都是整数)相除的结果是总是浮点类型
 大数可以使用_划线分组，比如 1_850_000 = 1850000
```
   
### 2.python中数学运算顺序
也就是说数学计算优先级
在python中的数值计算顺序与数学课本上的是一样的
- 1.指数运算最优先
- 2.再到乘除
- 3.加减

如果要改变以上规则，可以使用（）圆括号
比较一下以下两段程序输出的结果：
```py
rz = 2+3*5
print(rz)
```
```py
rz = (2+3)*5
print(rz)
```


### 3.在python中求余数的符号是什么
看看以下这段程序输出什么结果%号与/号的区别是什么
```py
rz = 10%3
print(rz)
```
### 4.在python中求次方的简化方式
    
```py
3*3*3*3*3 = 3**5
```

### 5.在python中的自增与自减的简单表达式
采用 +=号简写以下这段程序
```py
number_1 = 21
number_1 = number_1+1
```
采用 -=号简写以下这段程序
```py
number_1 = 21
number_1 = number_1-1
```

### 6.整数与浮点数的互换
将一个整数转换成浮点数，再将一个浮点数转换成整数

### 7.由字符串创建一个整数变量
提示：使用int(字符串)方法
由于字符串变量不能直接用来计算,所以如果一个数字是字符串，要在计算前应该将这个字符串转换成整数再做计算

### 8.由字符串创建一个浮点数变量，提示：使用float方法
如果字符串转换成整数的方法一样

### 9.已知速度与时间，求路程
已知一辆车的速度是每小时75.7 km, 他一个走了 6个小时，使用python求出这辆车一共走了多长的路程 

### 10.求某个天数内的分钟数
用户输入天数,比如1代表1天,2代表2天...然后求出相应天数的分钟数

### 11.乘号(*)的的特殊用法
*号还可以让字符串的本身变长多少倍
比如,让字符串'abc'变成'abc'+'abc'+'abc'...一直加到100

### 12.常见数学运行符

|操作符|名字|作用
|--|--|--|
`=` | 赋值 | 将一个值赋给一个名(变量) 
`+` | 加 | 两个数的相加，与可以用来连接字符串
`-` | 减 | 两个数相减
`+=` | 自增 | 将一个数加1 
`-=` | 自减 | 将一个数减1
`*` | 乘 | 两个数相乘
`/` | 除 | 两个数相除，如果两个数都是整数，结果只是整数商，而没有余数
`%` | 取余 | 得到两个数整除的余数
`**` | 求幂 | 将一个数自乘得到的结果，这个数及幂可以是整数或浮点数

# 五.流程控制语句之条件判断
程序中常见的流程控制有条件与循环两种语句
- 在学习之前要先了解代码块及其规范(:号与缩进)
- 任何对比的结果只有两个值(True,False,注意在python中True与False首字母都是大写)
- True为真，也就是符合条件
- False为假，也就是不符合条件

### 1.条件判断语句语法
条件判断语句分为单条件与多条件两种:
- 最基本的条件判断语句
```py
if 判断条件：
    执行语句……
else：
    执行语句……
```
- 当条件为多种可能值时，可以采用以下语法
```py
if 判断条件1:
    执行语句1……
elif 判断条件2:
    执行语句2……
elif 判断条件3:
    执行语句3……
else:
    执行语句4……
 
```
 

练习:
判断用户是否满18岁:
一种情况的判断
```py
age = input("请输入你的年龄: ")
age = int(age)
if age < 18:
    print("你是未成年人，不能玩游戏哦")
else:
    print(f"你今年{age}岁了，可以玩游戏，正在为你开启游戏，请稍等!")
```
多种情况的判断
```py
age = input("请输入你的年龄: ")
age = int(age)
if age < 3:
    print("你是在逗我吧!三岁小孩也能玩游戏")
elif age < 18:
    print("你是未成年人，不能玩游戏哦!")
elif age == 5:
    print("这里永远执行不到。")
elif age > 18:     
    print(f"你今年{age}岁了，可以玩游戏，正在为你开启游戏，请稍等!")
```

### 2.在条件判断中常用到的比较运算符
以下假设变量a为10，变量b为20：
| 运算符  | 说明  | 实例
|---|---|---| 
`==`	 | 等于 - 比较对象是否相等  |	(a == b) 返回 False。
`!=`  |	不等于 - 比较两个对象是否不相等  |	(a != b) 返回 True。
`>`	 | 大于 - 返回x是否大于y	 | (a > b) 返回 False。
`<`	 | 小于 - 返回x是否小于y。所有比较运算符返回1表示真，返回0表示假。这分别与特殊的变量True和False等价。注意，这些变量名的大写。	 |(a < b) 返回 True。
`>=`	 |大于等于 - 返回x是否大于等于y。	 |(a >= b) 返回 False。
`<=`	 |小于等于 - 返回x是否小于等于y。	 |(a <= b) 返回 True。

### 3.关于语句中的缩进是什么
- 每个条件后面要使用冒号 : 表示接下来是满足条件后要执行的语句块。
- 使用缩进来划分语句块，相同缩进数的语句在一起组成一个语句块。
### 4.如何表示a大于b
    > 习题：有一个游戏，只允许大于18岁的成年人才可以玩，应该怎么把这个关
### 5.如何表示a不等于b，
    > 提示:有两种表示方法
### 6.如何表示a大于18但是小50
> 小提示：这是采用范围比较
习题：有一个游戏，只允许大于18岁到50岁之间的成年人才可以玩，应该怎么把这个关

### 7.逻辑运算符
| 运算符  | 名字 |  实例 | 说明  |
|---|---|---|---| 
and | 与	| 	(a and b)  | a与b必须都为True才能达成条件
or	| 或者	|(a or b) | a与b其中有一个为True就可达成条件
not| 非，取反	| 	not a | 如果a为True即可是False,如果a为False即是True

练习:    
1)有一个游戏，只充值大于18岁到50岁之间的成年人才可以玩，应该怎么把这个关
> 小提示: 可以嵌套与可以使用and 

2)有一个游戏，只允许名字叫“小明”或“小强”或“小李”的人玩，应该怎么把这个关 

### 8.告诉用户输入的年份是否为闰年
要求用户输入一个年份，然后打印输出，这个年份是不是润年

```py
    year = int(input("输入一个年份: "))
    if (year % 4) == 0:
    if (year % 100) == 0:
        if (year % 400) == 0:
            print("{0} 是闰年".format(year))   # 整百年能被400整除的是闰年
        else:
            print("{0} 不是闰年".format(year))
    else:
        print("{0} 是闰年".format(year))       # 非整百年能被4整除的为闰年
    else:
    print("{0} 不是闰年".format(year))
```
***请理解以上示例，并自己动手写一遍***

# 六.流程控制语句之循环
我们的程序种要做重复性的劳动往往都是使用循环，
大多数程序中的循环都是有两种:
- 计数循环(for)
- 条件循环(while) 

###  1.理解一个简单的循环
```py
    for i in [1,2,3,4,5]:
        print('我叫小明')
```
> 小提示:我们要将很多个东西放到一个变量里时，需要采用中括号[]，不同的东西要使用逗号分开,其实也就是我们后面将学习到的另一种数据类型--列表类型

### 2.使用range()方法的作用
使用range()方法快速建立数值类型的列表
- Python3 range() 函数返回的是一个可迭代对象（类型是对象），而不是列表类型， 所以打印的时候不会打印列表。
- Python3 list() 函数是对象迭代器，可以把range()返回的可迭代对象转为一个列表，返回的变量类型为列表。
- Python2 range() 函数返回的是列表。
    
**range 语法如下：**
```py
    range(stop)
    range(start, stop[, step])

    # 参数说明：
    # start: 计数从 start 开始。默认是从 0 开始。例如range（5）等价于range（0， 5）;
    # stop: 计数到 stop 结束，但不包括 stop。例如：range（0， 5） 是[0, 1, 2, 3, 4]没有5
    # step：步长，默认为1。例如：range（0， 5） 等价于 range(0, 5, 1)
```

练习题：
使用range创建列表[1,2,3,4,5]
```py
    ls = list(range(5))
    print(ls)
    # 打印结果其实是:[0, 1, 2, 3, 4]
    # 想想为什么
```
注意： 
- range()方法 指定的范围是包含开始值，但不包含结束值
- range(0,5)的简写可以写成什么

想一想，以上的练习题应该怎么做才是正确的？
再想一想，为什么要使用range来构建列表？

### 3.什么是for循环变量
在循环过程中循环变量值发生什么变化
```py
    for i in range(0,5):
        print('我是',i)
```
> 注意观察每次循环后i的值的变化 
### 4.range的正向步长
练习:按2->100的顺序，输出100内的双数
### 5.range的反向步长
练习:按100->2的顺序，输出100内的双数


### 6.要求用户输入一个数字
然后依次输出由1到这个数据的乘法，比如用户输入3,那么要这样打印结果：
```py
1x3 = 3
2x3 = 6
3x3 = 9
```

### 7.循环非数值类型的列表
练习:有一个叫url的列表变量，保存了多个网址["www.baidu.com","www.163.com","www.qq.com","www.google.com","www.taobao.com"]，但是这些网址都少了https://，现在要给他们都加上https://应该怎么处理

```py
urls = ["www.baidu.com","www.163.com","www.qq.com","www.google.com","www.taobao.com"]
for url in urls:
    url = f'https://{url}'
    print(url)
```

### 8.跳出循环--break
练习: 有数值类型的列表[1,5,3,9,6]，采用for循环遍历这些数值，当遇到3的时候跳出循环
```py
numbers = [1,5,3,9,6]
for num in numbers:
    if num==3:
        break
    print(num)
```

### 9.你不合格下一个继续--continue
练习:有一个叫url的列表变量，保存了多个网址["www.baidu.com","www.163.com","www.qq.com","www.google.com",,"www.taobao.com"]，这些网址都少了https://， 现在要给他们都加上https://，不过www.qq.com不要加
```py
urls = ["www.baidu.com","www.163.com","www.qq.com","www.google.com","www.taobao.com"]
for url in urls:
    if url == 'www.qq.com':
        continue
    url = f'https://{url}'
    print(url)
```
 
### 10.循环的嵌套使用-妙用可变循环变量
 采用上层循环变量值
练习：采用for嵌套打印出九九乘法表，输出结果如下
    1x1=1    
    1x2=2    2x2=4    
    1x3=3    2x3=6    3x3=9    
    1x4=4    2x4=8    3x4=12    4x4=16    
    1x5=5    2x5=10    3x5=15    4x5=20    5x5=25    
    1x6=6    2x6=12    3x6=18    4x6=24    5x6=30    6x6=36    
    1x7=7    2x7=14    3x7=21    4x7=28    5x7=35    6x7=42    7x7=49    
    1x8=8    2x8=16    3x8=24    4x8=32    5x8=40    6x8=48    7x8=56    8x8=64    
    1x9=9    2x9=18    3x9=27    4x9=36    5x9=45    6x9=54    7x9=63    8x9=72    9x9=81

示例:
```py
for i in range(1, 10):
    for j in range(1, i+1):
        print(f'{j}x{i}={i*j}',end=' ')                
    print(' ')
```

### 11.条件循环while与for的区别
什么情况下使用for，什么情况下使用while
对于固定次数的情况下的循环 for 循环更加的好用
而对于不固定次数，或者次数不明的情况则使用 while 循环更加的方便。

### 12.使用while循环打印出10以内的整数
```py
num = 1
while num <= 9:
    print(num)
    num+=1 # 试想，如果将这句代码注释掉会是什么情况
```

### 13.用while循环打印出九九乘法表
类似10题，打印出九九乘法表，不过要求采用while嵌套实现
```py
row = 1
while row <= 9:
    col = 1
    while col <= row:
        print(f"{row}*{col}={row*col}", end = "  ")
        col += 1
    row += 1
    print() # 单纯的换行 
```


# 七.数据类型之列表
### 1.什么是列表
- 列表是一种容器(用来存储数据对象)
- 列表能够存储多个数据对象 - 序列
- 列表是一个可变序列
- 列表中的数据元素们会有先后顺序
### 2.如何创建一个空列表一非空列表
- 为什么有时要创建一个空列表
- 什么情况下创建非空列表

### 3.列表的分片操作
- 列表中元素的顺序是如何排列的
- 如何根据元素的顺序位置提取元素(也叫列表的分片)
- 在操作前理解正向索引与反向索引
值得注意的是，以下操作方式同样适合于字符串
下面以变量list_1为例：
```py
list_1 = ['red', 'green', 'blue', 'yellow', 'white', 'black']
```
练习1:通过list_1的索引提取出'blue' 主个元素
练习2:通过list_1的索引提取出'blue' 之后的所有元素，提示:常规写法与简化写法区别
练习3:通过list_1的索引提取出'blue' 之前的所有元素，提示:常规写法与简化写法区别
练习4:通过list_1的索引提同时取出['blue','yellow']
练习5: 采用反向索引提取出list_1的最后一个元素
练习6: 采用反向索引提取出list_1中倒数第三个元素
 
### 4.列表的更新与添加新项
有变量list如下：
```py
list_1 = ['red', 'green', 'blue', 'yellow', 'white', 'black']
```
练习1:修改list_1中的元素'yellow'将其变成'黄色'，打印list_1查看修改结果
练习2:给list_1追加一个元素，值是'orange'，打印list_1查看添加结果，提示：采用append函数
练习3:给list_1追加一个元素到'yellow'的前面，值是'orange'，打印list_1查看添加结果，提示：采用insert(索引，元素)函数
练习4:给list_1同时追加三个元素，值是['orange1','orange2','orange3']，打印list_1查看添加结果，提示：采用extend(元素列表)函数
### 5.列表元素的删除
常用三种删除法
- 已经知道元素的位置使用del(位置)
- 已经知道元素值使用remove(元素)
- 如果要获取某个元素，并将其从数组中删除使用pop,pop()不指定位置默认弹出最后一项,但也可以指定位置:pop(0)表示永远弹出第一项
有变量list如下：
```py
list_1 = ['red', 'green', 'blue', 'yellow', 'white', 'black']
```
练习1:采用列表索引，删除list_1中的'blue'项，提示：采用方法del
练习2:已知'blue'项，并在list_1中将其删除，提示：采用方法remove
练习3: 获取list_1最后一个元素，打印出其值，并将其从列表删除
练习4: 获取list_1第一个元素，打印出其值，并将其从列表删除
练习5: 看看以下程序，最终打印出来的结果是什么：
```py
colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
colors.insert(2,'蓝色')
item = colors.pop(0)
for i in range(len(colors)):
    item = colors.pop(0)
    print(item)
```

### 6.列表项的插入
练习在blue前插入一个蓝色
```py
    colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
    colors.insert(2,'蓝色')
    print(colors)
```

### 7.采用for循环遍历列表里的元素
要将取出一个列表里的元素，我们通常会使用for循环来操作，语法：
```py
for 元素 in 列表:
    print(元素)
```
看看以下程序打印了几次，每次打印的结果是什么
```py
colors = ['red', 'green', 1, 'yellow', 'white', 'black']
for item in colors:
    print(item)
```

### 8.采用for与range创建数值型列表
练习1:采用range创建一个[1,2,3,4,5] 的数值型列表
练习2:采用range加for创建一个[2,4,6,...,100] 的数值型列表,也就是100内的双数列表包括100,小提示： list_1 = [x*x for x in range(5)]

### 9.列表的排序
列表排序的方法有:
- 永久性排序使用 列表.sort() 或反向排序:列表.sort(reverse=True)
- 临时性排序使用 列表sorted(列表) 或反向排序:sorted(列表,reverse=True)

练习1:
数值列表的正向排序练习，将一个[3,1,0,2,4,5] 的数值型列表排序成[0,1,2,3,4,5]，小提示：采用sort()函数
     
练习2:
数值列表的逆向排序练习，将一个[3,1,0,2,4,5] 的数值型列表排序成[5,4,3,2,1,0]，小提示：采用.sort(reverse=True)
     
练习3:
字符串列表的正向排序练习，将一个["b","c","1","2","a","3",d","e","f"] 的数值型列表排序成['a','b','c','d','e','f']
     
练习4:
字符串列表的逆向排序练习，将一个["b","c","1","2","a","3","d","e","f"] 的数值型列表排序成['f','e','d','c','b','a']

### 10.将列表元素的顺序倒过来
要将列表中的元素倒转(注意不排序)可以使用
```py
列表.reverse()
```
练习:以下程序打印结果是什么
```py
colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
colors.reverse()
print(colors)
```
### 11.列表的常见操作
合并多个列表为一个列表可以采用+号
以下这个程序的打印结果是什么
```py
list_1 = [1, 2, 3]
list_2 = [4, 5, 6]
numbers = list_1 + list_2
print(numbers)
```
获取一个列表的长度(元素个数)可以使用len()方法
以下这个程序打印出来的值是多少
```py
colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
print(len(colors))
```
检查某个元素是否存在于列表可以使用in关键字
这个程序输出的结果是什么
```py
colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
print('red1' in colors)
```    
获取列表中的最大值用max()方法,获取列表最小值使用min()方法,这个操作一般用于数值型列表，如果字符串型的列表，将会是以首字母做为依据
以下三个程序分别输出的结果是什么
```py
nums = [1, 3, 5, 4, 7, 6]
print(max(nums))
```
```py
nums = [1, 3, 5, 4, 7, 6]
print(min(nums))
```
```py
colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
print(max(colors))
```
将列表转换成字符串使用'连接符号'.join(数组)
值得注意的是，join方法只能应用于纯字符数组
以下程序输出的结果是什么
```py
colors = ['red', 'green', 'blue', 'yellow', 'white', 'black']
print('_'.join(colors))
```
以下程序执行会报错吗，为什么
```py
colors = ['red', 'green', 1, 'yellow', 'white', 'black']
print('_'.join(colors))
```

### 12.元祖类型的创建
元祖与列表的操作是一样的，只不过创建的时候有所区别，列表采用中括号[]，而元祖采用小括号()
值得注意的是，元祖一旦创建后就不能改变，所以不能排序，不能删除，不能追加新项，由于元祖有不重复性，常这样将列表去重：
```py
results = ['a','b','c','a','b']
new_list = list(set(results))
```
### 13.列表中的列表
1.我们要收集三位同学(xiaoming,xiaoqiang,xiaoliang)的数学，语文，英语成绩，采用列表来收集应该怎么处理?
2.如何通过索引读取xiaoliang的语文成绩?
3.以上我们使用了程序中数据结构这个术语，数据结构是一种在程序中收集，存储或表示数据的方法，也就是数据的组织方式，被组织的数据可以是各种变量常量。



# 八.使用python控制硬件
本章以micobit这款编程版为示例
![](images/2021-11-10-16-03-33.png)
![](images/2021-11-10-16-04-06.png)
### 1.安装ide开发软件Mu Editor
Mu Editor 可以很好的与micobit配合，并以python语言来开发
 下载地址:https://codewith.mu/en/download
 下载后直接安装即可

### 2.连接micobit版，并显示123
使用可传输的数据的usb线连接micobit版到电脑，如果你的mu editor不是mic开发模式，会提示你是否切换到micobit开发模式，选择是即可
输出以下代码：
```py
    from microbit import *
    display.show(1)
    # display.show(123) 多个数字会轮流显示

```
    > 注:在每次写完代码后，都要注意一下检查，没有问题后，点击【刷入】将代码上传到micobit版里

    还可以，使用滚动的方式来显示:

```py
    from microbit import *
    display.scroll(1)
    # display.scroll(123) 多个数字会滚动显示出来
```
    可以尝试使用循环让他一直滚动下去

### 3.按钮事件监听
    当按下A键时，才显示123:
```py
    from microbit import *
    while True:
        if button_a.is_pressed():
            display.scroll(123)
```

### 4.当按下A键时一直显示一个心图
```py
    from microbit import *
    is_pre = False
    while True:
        if button_a.is_pressed():
            is_pre = True
        if is_pre:
            display.show(Image.HEART)
```

### 5.当按下B键时，关闭显示心图
```py
    from microbit import *
    is_pre = False
    while True:
        if button_a.is_pressed():
            is_pre = True
        if button_b.is_pressed():
            is_pre = False
            display.clear()
        if is_pre:
            display.show(Image.HEART) 

```

    练习:
    当我们按下A键时，micro:bit点阵就会显示一个箭头指向A键；当我们按下B键，micro:bit就会显示一个箭头指向B键；如果没有按键按下，micro:bit则显示一颗爱心
```py
    from microbit import *
    while True:
        if button_a.is_pressed():
            display.show(Image.ARROW_W)
        elif button_b.is_pressed():
            display.show(Image.ARROW_E)
        else:
            display.show(Image. HEART)
            display.clear()
```

### 6.让心跳动起来
    显示一个带有心跳的图片
```py
    while True:
        display.show(Image.HEART)
        sleep(500)
        display.clear()
        sleep(500)
```

### 7.自定义显示矩阵灯
点亮右上角那只灯:

```py
    ld = 1
    img = Image(
    "00009:"
    "00000:"
    "0000:"
    "00000:"
    "00000:"
    )
    display.show(img)
```
### 8.让led灯的亮度从0-9增加
```py
    from microbit import *
    while True:
        for i in range(10):        
            led = '00000:000{0}0:00{0}00:0{0}000:00000:'.format(i)
            img = Image(led)
            display.show(img)
            sleep(100)
```

### 9.使用led灯做一个动画效果
```py
    from microbit import *
    ripple1 = Image('00000:00000:00900:00000:00000:')
    ripple2 = Image('00000:00900:09690:00900:00000:')
    ripple3 = Image('00900:09690:96369:09690:00900:')
    ripple4 = Image('09690:96369:60006:96069:09690:')
    ripple5 = Image('96369:63036:30003:63036:96369:')
    ripple6 = Image('63036:30003:00000:30003:63036:')
    ripple7 = Image('30003:00000:00000:00000:30003:')
    ripple8 = Image('00000:00000:00000:00000:00000:')
    #创建列表
    ripple=[ripple1,ripple2,ripple3,ripple4,ripple5,ripple6,ripple7,ripple8]

    def showRipple(delay):
        while True:
            for i in ripple:
                display.show(i)
                sleep(delay)
            sleep(1000)

    if __name__=='__main__':
        showRipple(100) 
```

### 10.使用温度传感器显示当前温度
```py
    wan_du = temperature()
    while True:
    display.scroll(wan_du)
    sleep(1000) 
``` 

### 11.使用光线传感器控制灯的开关
```py
    from microbit import * 
    while True:
        if display.read_light_level() < 1:
            display.show(Image.HEART)
            sleep(100)
            display.clear()
            sleep(100)
        else:
            display.clear()
```

### 12.对与错
    学习单个引脚的使用，如果用鳄鱼夹夹住pin0引脚，鳄鱼夹的另一头夹住GND(也可以使用手指捏住两头),则micro:bit点阵会显示一个对，否则micro:bit点阵显示错:
```py
    while True:
        if pin0.is_touched():
            display.show(Image.YES)
        else:
            display.show(Image.NO)
```
    同学试试pin1脚

### 13.智能小车
- 点亮智能小车上的第一只灯
    ```py
        import neopixel
        display.show(Image.YES)
        # 定义流水灯接在引脚pin16上，数量为3个
        np = neopixel.NeoPixel(pin16, 3)
        np[0] = (255, 25, 25)
        np.show()
    ```
    练习点亮二只，第三只
- 循环显示，红，绿，蓝，RGB颜色：
    ```py
        from microbit import *
        import neopixel
        display.show(Image.YES)
        np = neopixel.NeoPixel(pin16, 3)
        # 红，绿，蓝
        led = [(255, 0, 0),(0, 255, 0),(0, 0, 255)]
        while True:
            for i in range(3):        
                np[i] = led[i]
                np.show()
                sleep(500)
                np.clear()
    ```

# 九.数据类型之字典
    字典与集合基本相同，本课程只讲字典类型，它们的唯一区别，就是集合没有键和值的配对，是一系列无序的、唯一的元素组合。
    字典是另一种可变容器模型，且可存储任意类型对象。 字典的每个键值 key=>value 对用冒号 : 分割，每个对之间用逗号(,)分割，整个字典包括在花括号 {} 中 ,格式如
    下所示：
    
```py
    dic_1 = {key1 : value1, key2 : value2, key3 : value3 }
```
- 1.创建一个字典用来保存一个同学的名字，年龄，班级
- 2.采用上面创建的字典，构建三个变量用来存放'来自五年级3班的小明11岁，来自五年级1班的小亮11岁，来自五年级2班的小明10岁'
- 3.将上面的三位置同学添加到列表，采用[列表项]方式或append的方式
- 4.通过循环打印输出列表中的所有同学字典对象
- 5.通过循环打印输出列表中的所有同学的姓名或年龄或班级
- 6.直接访问来自五年级2班的小明的年龄
- 7.检查五年级2班的小明的年龄是否存在(采用 in)，如果存在就将年龄修改成18岁 
- 8.采用for循环删除掉年龄大于11岁的同学(提示，请回顾列表的删除操作)

# 十.函数或方法
从现在开始，我们需要初步了解一下面向对象程序设计具有三大基本特征：封装、继承和多态。
函数是python中最小的封装单元,后面还有对象(类)，模块，包，库
本课程的着重讲函数，对象，模块
函数的定义方式：
```py
def 函数名（参数列表）:
    函数体
```
- 1.写一个无参函数，负责打印一行"==========================...",省略号代表有100个等号
- 2.写一个函数，要求有两个参数,这两个参数都接收一个数字,返回最大的数
- 3.写一个函数，要求输入一个数字，并返回这个结果是否负数还是正数
    > 提示:使用到if判断
- 4.写一个函数，传入一个数字，然后打印出来这个数字内的所有双数(偶数)
- 5.写一个函数,要求传入一个数字，然后依次输出由1到这个数据的乘法，比如用户输入3,那么要这样打印结果：
    ``` 
        1x3 = 3
        2x3 = 6
        3x3 = 9
    ```
- 6.如何给函数定使用文档
- 7.什么是传参数，什么是默认参数，什么是关键字参数
- 8.用函数做函数的参数
- 9.理解python中变量的作用域(局部变量与全局变量)
    > 注：python中的函数在调用时，会在内部创建所有使用到的变量，调用结束后会自动清除这些变量
    > 在函数内调用外部变量要注意的问题，
    - 1.读取时没有问题，可以正常读取
    - 2.如果要修改这个变量的值，将会重新创建一个变量副本，所以在外面的变量的值并不改变，
    - 3.想要在函数内改变外部变量的值，要使用global关键字的标识这个变量
    注意观察，下面两段程序的打印输出结果有什么不同
    
    程序1：
    ```py
        def printLine():
            global my_line
            my_line = "==="
            print(my_line)

        my_line = "="
        printLine()
        print(my_line)
    ```
    程序2：
    ```py
        def printLine():
            global my_line
            my_line = "==="
            print(my_line)

        my_line = "="
        printLine()
        print(my_line)
    ```

# 十一.类与对象
类与对象与对象在面向对象编程语言中非常重要，所以这章会讲的篇幅比较大
- **1.什么是类，什么是对象**
    > 1)对象=属性+方法,理解对象中的属性与方法
    > 2)对象的模板是类
    > 3)对象有什么特性与方法处决于类提供了什么样的属性与方法,不过属性也可以在后期追加,不建议这样做，应该在设计类时就决定好这类对象的属性与行为


- **2.对象模板的设计(类)**
    > 1)理解类中的特殊方法__init__与__str__，注意，特殊方法前后分别有两个下划线
    > 2)在设计一个类时，是不是必须要有__init__初始化方法
    > 3)类的方法与self关键字的关系
    > 4)什么是对象的属性
    > 5)如何通过__init__方法中初始化对象(实例)属性
    > 6)类的动作或者说类的功能，也叫类的方法，如何定义

    看看下面这个类示例,理解其结构,这是定义了一个用户玩游戏的类，要求满18岁才可以玩:

    ```py

    class User: 

        def __init__(self, user_name, user_age):
            self.name = user_name
            self.age = user_age
            self.age_min = 18

        def play(self):
            if self.age < self.age_min:
                print(f'{self.name}你还没满{self.age_min}岁，不能玩这个游戏哦！')
            else:
                print(f'{self.name}游戏开始了...')

    ```

- **3.什么是对象的实例,如何创建一个实例**
    如对上面那个类，创建一个xiao_cai的实例:
    ```py
    xiao_cai = User("小菜", 17)
    ```


- **4.类的属性与实例（对象）属性有什么区别**
    > 1)类的属性可以直接使用类名加.来调用，不需要创建实例，对象的属性必须要通过对象来调用
    > 2)当采用实例来调用类属性时，类属性也可以像实例属性一样使用,但
    > 3)可以看出，类属性更适合定义一些不变的常量，或者说适合所有类都会共同使用的到的变量,可以理解为类的共享字段

    示例：定义一个用户玩游戏的类，但是要满一定的年龄的人才可以玩，
    这个年龄限制默认是18岁，但我们也可以改变它，并且这个改变要影响所有玩游戏的人，所以这个年龄限制设计成类属性比较适合

    ```py

    class User:
        ageMin = 18

        def __init__(self, user_name, user_age):
            self.name = user_name
            self.age = user_age

        def play(self):
            if self.age < self.ageMin:
                print(f'{self.name}你还没满{self.ageMin}岁，不能玩这个游戏哦！')
            else:
                print(f'{self.name}游戏开始了...')

    ```

    观察一下，以下调用变化：

    ```py
    User.ageMin = 21  # 如果有一天，我们不想采用默认的18岁，我们可以这样修改这个年龄限制,这个改动将影响到下面所有的实例

    xiao_cai = User("小菜", 17)
    xiao_cai.play()

    xiao_cheng = User("小陈", 20)
    xiao_cheng.play()
    ```

    > 可以看出，类属性非常适合不同实例共享变量或常量，不过，如果你要让实例来调用类属性也是可以的，不过最好统一规范，实例的变量直接在实例init的时候创建，这样，在实例用完后会自动清理

- **5.类的访问限制**
    有时我们不希望向调用者暴露某些方法与属性, 比如上面的那个用户玩游戏的类，目前我们可以通过实例来调用用户的姓名与年龄：
    ```py
    xiao_cai = User("小菜", 17)
    print("姓名：", xiao_cai.name)
    print("年龄：", xiao_cai.age)
    ```
    现在我要改造一下这个类，让年龄不能在外面调用，只允许在类的内部调用
    同时，我还将判断是否可以允许用户玩游戏的业务处理提出来，放到一个方法中
    并且这个方法也只能在类的内部调用，外部不能调用：
    ```py
    class User:
        ageMin = 18

        def __init__(self, user_name, user_age):
            self.name = user_name
            self.__age = user_age

        def play(self):
            if self.__isAllow():
                print(f'{self.name}你还没满{self.ageMin}岁，不能玩这个游戏哦！')
            else:
                print(f'{self.name}游戏开始了...')

        def __isAllow(self):
            return self.__age < self.ageMin
    ```
    这个时间，如果你调用__age属性与__isAllow方法就会报错:
    ```py
    xiao_cai = User("小菜", 17) 
    print("年龄：", xiao_cai.__age)
    ```
    我只是在属性与方法前面加了两个下划线，就实现了属性与方法的外部访问限制
    > 总结，要禁止类中的属性或方法被外部调用，可以在属性或方法前面加双下划线

- **6.类的多态与继承**
    面向对象(OOP)有两个非常重要的知识点，就是多态与继承
    >1) 多态：简单的说，多态就是同一个方法，有不同的行为,也就是说对于不同的类，有着共同的方法，只不过相同的方法里要做的事情不一样

    比如，上面玩游戏的类，默认情况下，他们只能玩同一款游戏，现在有两款游戏可以让他们玩，所以要设计两个类，但是这两个类又有着很多共同点（比如，用户的姓名，用户的年龄，判断用户是否适合玩游戏的条件），如果说每个类都写一遍这些共同点，那也太麻烦了，并且以后如果有几百款游戏呢，其不是要写几百次，如果我些共同点里面，有那个地方要修改了，那就要修改几百个类，想想这太可怕了，好在类的多太与给我们很的解决了这个问题
    我们要解决这个问题之前，我还要了解一下继承

    >2) 继承
    实现生活中就有传宗接代，儿子继承了父母的很多特性，类也可以这样，将共同的地方留给父类去做，不同的地方让子类去做    
    比如我们现在要让用户玩两款游戏，一款叫《我的世界》另一个叫《和平精英》
    《我的世界》我们给他起个类名叫 Game1,和平精英叫 Game2,我们的父类叫:GameBase,现在改造一下，上面的类:
    
    ***先看你类GameBase的设计***
    > 理解父类的共性设计原理,注意pass的占位应用或raise异常的应用
    ```py
    class GameBse:
        ageMin = 18

        def myGame(self):
            raise Exception('子类中必须实现该方法') # 也可以采用pass

        def __init__(self, user_name, user_age):
            self.name = user_name
            self.__age = user_age

        def play(self):
            if self.__isAllow():
                print(f'{self.name}你还没满{self.ageMin}岁，不能玩这个游戏哦！')
            else:
                self.myGame()

        def __isAllow(self):
            return self.__age < self.ageMin
    ```
    ***设计玩《我的世界》的子类***
    >我们只要在子类里重写myGame这个方法，并在这个方法启动《我的世界》这款游戏即可
    ```py
    class Game1(GameBse):
    def myGame(self):
        print(f"我是{self.name},我正在玩《我的世界》")
    ```

    ***设计玩《和平精英》的子类***
    >我们只要在子类里重写myGame这个方法，并在这个方法启动《和平精英》这款游戏即可
    ```py
    class Game1(GameBse):
    def myGame(self):
        print(f"我是{self.name},我正在玩《我的世界》")
    ```

    > 看看我们的这两个子类的代码是不是很简洁呢

    调用示例：
    ```py
        GameBse.ageMin = 21  # 如果有一天，我们不想采用默认的18岁，我们可以这样修改这个年龄限制,这个改动将影响到下面所有的实例

        # xiao_cai = GameBse("小菜", 17) # 抽象类不能被实例化，这样创建将会报错
        xiao_cai = Game1("小菜", 21)
        xiao_cai.play()

        xiao_cheng = Game2("小陈", 21)
        xiao_cheng.play()
    ```
    > 总结: 在python中只要子类编写了与父类同名方法，父类的方法将会被子类覆盖,这就是多态

- **7.抽象类**
    本次教程并不打算讲抽象类，因为在python中，并且抽象类在python中的体现好像不是那么重要，不过其他语言经常使用，所以这里还是简单讲讲
    > 1)抽象类不能实例化，在python中如果调用抽象类来创建实例，一样会引发错误
    > 2)python中也没有接口，可以采用抽象类来实现
    > 3)python中使用抽象类的好处在于可以约束子类必须实现指定的抽象方法


    实现抽象类只需要两步:
    > 1)让类继承于ABC类
    > 2)类中要有@abstractmethod注解的方法

    如将上面的父类实现成抽象类:

    ```py
    class GameBse(ABC):
    ageMin = 18

    @abstractmethod
    def myGame(self):
        pass

    def __init__(self, user_name, user_age):
        self.name = user_name
        self.__age = user_age

    def play(self):
        if self.__isAllow():
            print(f'{self.name}你还没满{self.ageMin}岁，不能玩这个游戏哦！')
        else:
            self.myGame()

    def __isAllow(self):
        return self.__age < self.ageMin
    ```

    > 注：上面的这个类，可以直接实例化吗

# 十二.模块
1.想想我们生活中什么是模块化的
2.如果说python中函数是最小的积木，那么类就是一组积木，那么我们现在讲的模块则是一桶积木
3.模块就是一个python文件
4.如何引用整个模块（或者说一个py文件）,提示：使用关键争import
5.如何引用模块中的某个特性，也就说模块说的某个方法，类...，提示: 使用from ... import
6.如何一次性导入所有的特性，不建议这样做，为什么
7.偿试调用python内置的模块，time,random
8.偿试安装第三方模块，并调用第三方模块，以MyQR为例子,生成一个带动态图的二维码:
```py
from MyQR import myqr
 
myqr.run(words="http://www.baidu.com", picture="霹雳布袋戏.gif", colorized=True)
# 动态图要使用gif格式的图片
# words参数是指定二维码的内容
# picture参数是指定要使用的图片文件名，这里的图片是在与这个python文件所属的目录下
# colorized参数是指定生成的二维码图片是彩色的，如果为False或者不设置生成的图片是黑白色的
```





