---
date: 2026-09-19
aliases:
  - python基础语法
---
---

#### 第一个hello world

```python
print("hello word" )
```
没错就这么简单，相较于c/c++来说实在是太简单了 不需要声明数据类型 ，也不用写复杂的头文件 也不用写main函数以及return啥的 ,甚至每行不用”；“      码量起码减少一半 ，难怪python是最是适合做开发的语言

-  #  代表注释也比c方便  ctrl加/可以批量注释

  现在我已经决定以后项目都用python了


---

### 字面量类型以及书写格式

和c差不多只有空值我不知道
- 空值（None  Type）———— None

```python
#他甚至可用true·加1
print(True+1)
#注意T要大写 只有True才是python库里的
```

- 要注意有""的都是字符串因此比如“10010”与10010 是两个不一样的类型
- “True”与True也不一样‘


---
### 变量

###### 要注意变量是指存储数据的容器（空间），而非容器里的数据

----

- 定义格式：变量名=变量的值   num=11265 很简单 连类型都是动态的num甚至可以=shit

```python

apple=100
grape=5255

print("苹果和葡萄一共：" ,apple+grape)

```

---

#### 标识符

一、什么是标识符
标识符就是你自己起的名字，用来表示：

变量名：apple、grape

函数名：print、add

类名：Person

模块名：math

常量名：PI

----


二、Python 标识符的硬性规则
和 C/C++ 类似，但更宽松：

- 只能包含：字母、数字、下划线 _

- 不能以数字开头

- 区分大小写：apple 和 Apple 是两个不同的名字

- 不能是关键字：if、for、class、def、return 等

- 不能包含空格、-、@、# 等符号
----
### 关键字

False      None       True       and        as
assert     async      await      break      class
continue   def        del        elif       else
except     finally    for        from       global
if         import     in         is         lambda
nonlocal   not        or         pass       raise
return     try        while      with       yield

---
### 字符串

#双引号
s1 =  “hello”

 #单引号 
s2 = 'hello'

#三引号

s3 = """      """

- 转译:  当你要写比如it‘s那单引号会与it's中的’  先组成一组单引号 因此用转义字符
-  加一个"/"转译即可
- 或你直接有双引号也行

----
### 字符串拼接
```python
slogan="问剑""白玉京"

slogan="问剑"+"白玉京"
#可以直接加
```

人生苦短，我用python


- 可以用占位符完成字符串和变量的快速拼接（其中%表示我要占位）
```python
name="问剑白玉京"
print("大家好，我是%s，欢迎大家"%name)


s1=l

s2=yue

print("我是%s,他是%s"%s(s1,s2))
```
---

### 字符串格式化

也可以通过f“内容{变量、表达式}”的形式来完成快速格式化

```python
name="问剑白玉京"
print(f"大家好，我是{name}，欢迎大家")
```

##### 这个应该是最推荐的写法

-----

### 输入与输出

**input**和**print**


