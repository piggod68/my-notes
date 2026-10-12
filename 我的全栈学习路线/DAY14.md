---
date: 2026-10-06
aliases:
  - 函数
---
----

```python
#计算园的函数
def calculate_circle_area(radius):
    area = 3.14 * radius ** 2
    return area
area_1 = calculate_circle_area(5)
print(f"半径为5的圆的面积为: {area_1}")
```

---

## 需要接受两个变量

```python
##长方形
def rectangle_area(length, width):
    """计算矩形的面积"""
    return length * width
print(rectangle_area(5, 3))
```

-----

## 返回多个返回值

```python
 def circle_area_len(radius):
    return 3.14 * radius ** 2,  round(2*3.14 * radius,1)
al=circle_area_len(5)
print(al)
# 输出(78.5, 31.4)
#多个返回值可以用元组的形式返回，调用时也可以用元组接收。
```
----

# 函数的说明文档

#### 它其实就是在函数内部的第一行，用三个双引号 """ 包裹起来的一段文字

```python
def add(a, b):
    """
    这里是函数的说明文档。
    这个函数的作用是计算两个数字的和。
    """
    return a + b
```


### 为什么不用#

# 注释：只是写给“人”看的，Python 解释器在运行时会直接忽略它。

说明文档（Docstring）：它是写进函数内存里的！Python 会把它当成函数的一个属性保存起来（函数名.__doc__）。

这就意味着你可以用代码把说明文档打印出来


----
一句话描述：这个函数是干嘛的。

- Args: (参数)：每个参数的名字、类型、含义

- Returns: (返回值)：函数返回什么，类型是什么

- Raises: (异常)：什么情况下这个函数会报错（可选）
---
```python
def rectangle_area(length, width):
    """
    计算矩形的面积
    :param length: 矩形的长度
    :param width: 矩形的宽度
    :return: 矩形的面积
    """
    return length * width
```

-----

# 函数的嵌套
