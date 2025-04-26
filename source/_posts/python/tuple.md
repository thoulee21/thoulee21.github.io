---
title:  Python 元组(Tuple) 练习题
date:   2021-06-01 16:27:32
categories:
  - Legacy
  - Python
tags:
  - Python
  - Study
---

# Python 元组(Tuple) 练习题

## 1. 将一个给定的整型元组：`tuple(range(1, 7))`倒序输出

```python
nums = tuple(range(1, 7))

print(nums)
# (1, 2, 3, 4, 5, 6)
```

```python
list_nums: list = sorted(nums, reverse=True)
tuple_nums = tuple(list_nums)

print(list_nums)
print(tuple_nums)
```

```shell
[6, 5, 4, 3, 2, 1]
(6, 5, 4, 3, 2, 1)
```

## 2. 请问以下变量哪些是 `tuple` 类型：  
> A. a = ()  
> B. b = (1)  
> C. c = [2]  
> D. d = (3,)  
> E. e = (4, 5, 6)

```shell
A, D, E
```
