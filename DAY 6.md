---
date: 2026-09-20
aliases:
  - python语法
---
-----

### 输入输出


**就是cin   cout**

```python
name=input("输入名字；")

print(f"你的名字是{name}")
```


---

#### 运算符

-  整除： /
-  幂指数：**          10 ** 3 = 10的三次方



```python
x=int(input())
y=int(input())
result1=x+y
result2=x-y
print(f"x+y={result1}")
print(f"x-y={result2}")
```


----

赋值运算和比较都和c一样

----




#### if语句其实差不多就是跟简单

```python
score = 85
if score >= 90:          # 没有括号，结尾有冒号
    print("优秀")         # 缩进 4 个空格，代表属于 if 的代码块
elif score >= 60:        # Python 中是 elif，不是 else if
    print("及格")
else:
    print("不及格")
```

