---
date: 2026-10-05
aliases:
  - 字典，函数
---
----
# 字典 (Dictionary)

- 字典：使用键值对（key: value）来存储数据，每一个键都对应一个值，通过键（key）可以快速找到对应的值（value）。
- 特点：键值对（key: value）存储、键（key）不能重复、可修改。

## 定义：

```python
# 定义字典
字典名称 = {key: value, key: value, key: value ...}

# 定义空字典
字典名称 = {}
字典名称 = dict()

# 根据key获取value
值 = 字典名称[key]
```
## 一一对应

---
## 获取

- 就是直接用`x`=dict[""]

----
| 类型 | 操作 | 含义 | 样例 |
| :---: | :--- | :--- | :--- |
| **添加** | `字典名称[key] = value` | 往指定字典中添加key-value键值对 | `dict1["涛哥"] = 688` |
| **删除** | `字典名称.pop(key)` | 删除字典中指定的key，并返回该key对应的value | `score = dict1.pop("涛哥")` |
| | `del 字典名称[key]` | 删除字典中指定的键值对 | `del dict1["涛哥"]` |
| **修改** | `字典名称[key] = value` | 修改字典中指定的key对应的值 | `dict1["小智"] = 658` |
| **查询** | `字典名称[key]` | 根据key获取value | `dict1["涛哥"]` |
| | `字典名称.get(key)` | 根据key获取value | `dict1.get("涛哥")` |
| | `字典名称.keys()` | 获取所有的key | `dict1.keys()` |
| | `字典名称.values()` | 获取所有的value | `dict1.values()` |
| | `字典名称.items()` | 获取所有的key-value键值对 | `dict1.items()` |

----


# 函数

## 很白话就是def 调用就是 out_line

```python
# C 语言写法：
# int add(int a, int b) { return a + b; }

# Python 写法：
def add(a, b):          # def 开头，没有类型
    result = a + b      # 缩进 4 格
    return result       # 返回

# 调用
x = add(3, 5)
print(x)  # 输出 8
```



