# 30天Python编程挑战 -- 第3天 :triangular_flag_on_post:

> 本项目翻译自[Asabeneh/30-Days-Of-Python](https://github.com/Asabeneh/30-Days-Of-Python)，并稍作修改，如有需要请参考原项目并支持原作者。

:pushpin:项目本意是为了家人和身边的朋友快速了解Python编程。:clown_face:请勿随意转载/发布。

:speech_balloon:可添加微信：xumaimeng，:label:备注：挑战python，获取帮助。



---

[TOC]

---



## 布尔值

布尔数据类型只有两个值：**True**和**False**。当我们在使用比较运算符的时候，返回的结果就是一个布尔值。

```python
print(True)
print(False)
```



## 运算符

Python支持很多类型的运算符，我们先来学习其中几个。



### 赋值运算符

赋值运算符顾名思义是对变量进行赋值。我们以`=`为例，数学中的等号代表两个数值相等，在Python中，等号意味着将值赋给一个变量，我们称为赋值或是给变量赋值。下面来看一下有哪些赋值运算符：

| 运算符 | 写法一  | 写法二     |
| ------ | ------- | ---------- |
| =      | x = 5   | x = 5      |
| +=     | x += 5  | x = x + 5  |
| -=     | x -= 5  | x = x - 5  |
| *=     | x *= 5  | x = x * 5  |
| /=     | x /= 5  | x = x / 5  |
| %=     | x %= 5  | x = x % 5  |
| //=    | x //= 5 | x = x // 5 |
| **=    | x **= 5 | x = x ** 5 |
| &=     | x &= 5  | x = x & 5  |
| \|=    | x \|= 5 | x = x \| 5 |
| ^=     | x ^= 5  | x = x ^ 5  |
| >>=    | x >>= 5 | x = x >> 5 |
| <<=    | x <<= 5 | x = x << 5 |



### 算术运算符

- 加法（+）：a + b
- 减法（-）：a - b
- 乘法（*）：a * b
- 除法（/）：a / b
- 取余（%）：a % b
- 整除（//）：a // b
- 指数（\*\*）：a \*\* b

例子：整数

```python
# Python算术运算符
# 整数

print('加法：', 1 + 2)
print('减法：', 2 - 1)
print('乘法：', 2 * 1)
print('除法：', 3 / 2)
print('整除：', 3 // 2)
print('取余：', 3 % 2)
print('指数：', 3 ** 2)    # 3的平方，=3*3
```



例子：浮点数

```python
# 浮点型数据

print('pi 值：', 3.14)
```



例子：复数

```python
# 复数

print('复数：', 1+1j)
print('复数乘法：', (1+1j)*(1-1j))
```



现在来声明一些变量并给变量赋值。我这里使用了一些单字符来声明，实际开发中不能这么使用，我们一定要使用好记的变量名。

例子：

```python
# 在开头进行变量声明

a = 3    # 有个变量叫a，赋值了一个数值型数据3
b = 2    # 变量b赋值了整数2

# 将变量计算后的结果赋值给新的变量
total = a + b
diff = a - b
product = a * b
division = a / b
remainder = a % b
floor_division = a // b
exponential = a ** b

# 上面的total变量本改使用sum单词，但是sum是Python内建函数，应该避免和它冲突
print(total) # 直接打印结果有可能不记得这个值是怎么来的，所以一般会拼接一些辅助字符，像下面这些
print('a + b = ', total)
print('a - b = ', diff)
print('a * b = ', product)
print('a / b = ', division)
print('a % b = ', remainder)
print('a // b = ', floor_division)
print('a ** b = ', exponentiation)
```



例子：

```python
print('== 算术运算 ==')

# Declaring values and organizing them together
num_one = 3
num_two = 4

# Arithmetic operations
total = num_one + num_two
diff = num_two - num_one
product = num_one * num_two
div = num_two / num_one
remainder = num_two % num_one

# Printing values with label
print('total: ', total)
print('difference: ', diff)
print('product: ', product)
print('division: ', div)
print('remainder: ', remainder)
```



我们开始使用已经学会的这些知识，进行一些简单的计算。

例子：

```python
# 计算圆的面积
radius = 10                                 # 圆的半径
area_of_circle = 3.14 * radius ** 2         # 两个*代表指数运算
print('Area of a circle:', area_of_circle)

# 计算矩形面积
length = 10
width = 20
area_of_rectangle = length * width
print('Area of rectangle:', area_of_rectangle)

# 计算物体重力
mass = 75
gravity = 9.81
weight = mass * gravity
print(weight, 'N')                         # 给打印的重力加一个单位
```



### 比较运算符

在Python中比较两个数值的大小通常会使用比较运算符，下表展示了Python中拥有的比较运算符和使用例子。

| 操作符 | 名称     | 例子   |
| ------ | -------- | ------ |
| ==     | 等于     | x == y |
| !=     | 不等于   | x != y |
| >      | 大于     | x > y  |
| <      | 小于     | x < y  |
| >=     | 大于等于 | x >= y |
| <=     | 小于等于 | x <= y |



关于比较运算符的一些例子：动手试一试

```python
print(3 > 2)     # True, because 3 is greater than 2
print(3 >= 2)    # True, because 3 is greater than 2
print(3 < 2)     # False,  because 3 is greater than 2
print(2 < 3)     # True, because 2 is less than 3
print(2 <= 3)    # True, because 2 is less than 3
print(3 == 2)    # False, because 3 is not equal to 2
print(3 != 2)    # True, because 3 is not equal to 2
print(len('mango') == len('avocado'))  # False
print(len('mango') != len('avocado'))  # True
print(len('mango') < len('avocado'))   # True
print(len('milk') != len('meat'))      # False
print(len('milk') == len('meat'))      # True
print(len('tomato') == len('potato'))  # True
print(len('python') > len('dragon'))   # False


# Comparing something gives either a True or False

print('True == True: ', True == True)
print('True == False: ', True == False)
print('False == False:', False == False)
print('True and True: ', True and True)
print('True or False:', True or False)
```



Python中还有几个特殊的比较运算符：

- is：当两个变量值相同时返回True（x is y）
- is not：当两个变量值不相同时返回True（x is not y）
- in：判断两个变量的包含关系，如果a是b的子集，返回True（a in b）
- not in：判断两个变量的包含关系，如果a不是b的子集，返回True（a not in b）



```python
print('1 is 1', 1 is 1)                   # 返回True - 因为这俩值是一样的
print('1 is not 2', 1 is not 2)           # True - 
print('A in Asabeneh', 'A' in 'Asabeneh') # True - 因为字符串中有A
print('B in Asabeneh', 'B' in 'Asabeneh') # False - 因为字符串中没有B
print('coding' in 'coding for all') # True - 因为coding for all中有单词coding
print('a in an:', 'a' in 'an')      # True
print('4 is 2 ** 2:', 4 is 2 ** 2)   # True
```



### 逻辑运算符

Python中使用关键词**and**、**or**、**not**来作为逻辑运算符。逻辑运算符一般用来组合多个条件语句。

| 操作符 | 解释                                                       | 例子                  |
| ------ | ---------------------------------------------------------- | --------------------- |
| and    | **与**运算，当所有条件都为True时，返回True，否则返回False  | x < 5 and x < 10      |
| or     | **或**运算，当所有条件都为False时，返回False，否则返回True | x < 5 or x < 4        |
| not    | **非**运算，反转条件的结果                                 | not(x < 5 and x < 10) |



试一试

```python
print(3 > 2 and 4 > 3) # True - 因为两个条件都是True
print(3 > 2 and 4 < 3) # False - 因为第二个条件为False
print(3 < 2 and 4 < 3) # False - 两个条件都为False
print(3 > 2 or 4 > 3)  # True - 两个条件都是True
print(3 > 2 or 4 < 3)  # True - 有一个条件是True
print(3 < 2 or 4 < 3)  # False - 两个条件都是False
print(not 3 > 2)     # False - 因为 3 > 2 为 true, 然后 not True 即 False
print(not True)      # False 
print(not False)     # True
print(not not True)  # True
print(not not False) # False
```



## 练习

1. 声明你的年龄（age）为整型变量

2. 声明你的身高（height）为浮点型变量

3. 声明一个复数变量

4. 编写一段代码，运行后可以分别键盘输入一个矩形的长和宽，然后计算矩形的面积，过程如下：

   ```python
   Enter base: 20		# 先输入一个值
   Enter height: 10  # 再输入一个值
   The area of the triangle is 100   # 计算乘积
   ```

   

5. 编写一段代码，键盘输入得到矩形的长和宽，计算矩形的面积和周长

6. 编写一段代码，键盘输入得到圆的半径，计算圆的面积和周长

7. 尝试计算y值(y = x^2 + 6x + 9)，尝试不同的x来输出y，并找出使y等于0的x值

8. 计算`‘python’`和`‘jargon’`的长度，并比较两个值，看结果为True还是False

9. 尝试比较一下`‘10’`和10的值是否相同

10. 编写一段代码，使运行后打印如下数列

    ```python
    1 1 1 1 1
    2 1 2 4 8
    3 1 3 9 27
    4 1 4 16 64
    5 1 5 25 125
    ```

    

