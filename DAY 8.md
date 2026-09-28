---
date: 2026-09-22
aliases:
  - 依旧沉淀语法基础
---
# Python 笔记：`print()` 中的 `end=""` 参数详解

## 1. 核心作用
`end=""` 的作用是：**告诉 Python，打印完当前内容之后，不要自动换行。**

## 2. 默认规则 vs 使用 `end=""`

### 🔴 默认情况：自动换行
在 Python 中，`print()` 函数默认会在打印内容的末尾加上一个**换行符 (`\n`)**。
你可以把 `print("A")` 等同于 `print("A", end="\n")`。

**代码演示：**
```python
print("A")
print("B")
print("C")
```


打印结果就是竖着的 他每一个都会自动换行
A
B
C

而加了 end=“” 
就是横着的ABC

# 嵌套循环

```python
   for i in range(m):          # 外层循环：控制行数
    for j in range(n):      # 内层循环：控制每一行打印几个星星
        print("*", end="")  # 关键在这里！
    print()                 # 这一行专门用来换行
```



### 乘法表

```python
for i in range(1,10):
    for j in range(1,i+1):
            print(f"{i}*{j}={i*j}", end="\t")#\t表示制表符，\n表示换行
    print()
```


## 循环案例

```python
import random

random_number=random.randint(1, 100)

num=int(input("请输入一个1-100之间的数字："))

  

while num != random_number:

    if num < random_number:

        print("你猜的数字小了，请重新输入")

    else:

        print("你猜的数字大了，请重新输入")

    num=int(input("请输入一个1-100之间的数字："))

print(f"恭喜你，猜对了，数字是{random_number}")
```


-----


# Python 核心数据储存容器（四大收纳工具）

## 为什么需要容器？
在编程中，我们不可能只处理一两个数据。如果我们要处理全班 50 个学生的名字，总不能写 50 个变量（`name1`, `name2`...）吧？这时候就需要**数据储存容器**。

你可以把容器想象成生活中的收纳工具：有的像抽屉（有顺序），有的像带标签的收纳盒（按键找东西），有的像密封罐（放了就不能改）。

Python 中最常用的四大核心容器是：**列表（List）、元组（Tuple）、字典（Dictionary）、集合（Set）**。

---


