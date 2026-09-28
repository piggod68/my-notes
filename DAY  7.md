---
date: 2026-09-21
aliases:
  - 依旧在python语法
---
## if
-----
```python
a=int(input("请输入第一条边： "))
b=int(input("请输入第二条边： "))
c=int(input("请输入第三条边： "))

if a+b>c and a+c>b and c+b>a :
   # pass    #pass为空语句 就是等会来写 只是为了结构的完整
    if  a==b and b==c:
        print(f"{a}{b}{c}构成等边三角形~")
    elif a==b or b==c or a==c:
        print(f"{a}{b}{c} 这三个边构成等腰三角形~")
    else :
 
       print(f"{a},{b},{c}这三条边构成普通三角形~")
else:
    print(f"{a}{b}{c}这三个边可以构成三角形")
```



---
## 结构模式匹配

- 就是匹配match case

```python
day = input("请输入今天是星期几：")

  

match day:

    case "1":

        print("今天是星期一")

    case "2":

        print("今天是星期二")

    case "3":

        print("今天是星期三")

    case "4":

        print("今天是星期四")

    case "5":

        print("今天是星期五")

    case "6":

        print("今天是星期六")

    case "7":

        print("今天是星期日")

    case _:

        print("输入有误，请输入1-7之间的数字")
```



----



### 简易计算器
```python
num1=int(input("请输入第一个数字："))

num2=int(input("请输入第二个数字："))

operator=input("请输入运算符（+、-、*、/）：")

  

match operator:

    case "+":

        print(f"{num1}+{num2}={num1+num2}")

    case "-":

        print(f"{num1}-{num2}={num1-num2}")

    case "*":

        print(f"{num1}*{num2}={num1*num2}")

    case "/" if num2 != 0:  #还能再case后面有if太夯了
    

        print(f"{num1}/{num2}={num1/num2}")

    case _:

        print("输入有误，请输入正确的运算符")
```

他哥的python真的简洁 好用 好学 最接近自然语言的
python nb

----
## 循环

### while

```
while 条件表达语句：
     循环语句1
     循环语句2
else
```

```python
i=0
while i<10:
    print(f"人生苦短，我用Python")
    i+=1
else:
    print("循环结束")
```

---

### for

```python
  for 元素  in 待处理数据集；
     
  else；
   循环结束时，执行的代码
```


```python

range语句

range（5）就可以得到01234

range（end）就是从0到end-1

range（start，end，step）
比如：
range（0，10,2）——————0,2，4,8
```

