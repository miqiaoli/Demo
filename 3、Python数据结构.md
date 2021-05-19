# Python数据结构

## 一. 常见的数据结构:
- 堆栈（Stack）
- 队列（Queue）
- 数组（Array）
- 链表（Linked List）
- 树（Tree）
- 图（Graph）
- 堆积（Heap）
- 散列表（Hash table）

## 二. 列表
```python
>>> a = [23, 45, 1, -3434, 43624356, 234]
>>> a.append(45)
>>> a
[23, 45, 1, -3434, 43624356, 234, 45]
```
##### 1. `insert()` ---- 将数据插入到列表的任何位置
```python
>>> a.insert(0, 1) # 在列表索引 0 位置添加元素 1
>>> a
[1, 23, 45, 1, -3434, 43624356, 234, 45]
```

##### 2. `count(s)` ---- 返回列表中元素s的数量
```python
>>> a.count(45)
2
```

##### 3. `remove(s)` ---- 删除列表中元素s
```python
>>> a.remove(234)
>>> a
[111, 1, 23, 45, 1, -3434, 43624356, 45]
```

##### 3. `reserve()` ---- 反转整个列表
```python
>>> a.reverse()
>>> a
[45, 43624356, -3434, 1, 45, 23, 1, 111]
```

##### 3. `a.extend(b)` ---- 将列表b添加到a的末尾
```python
>>> b = [45, 56, 90]
>>> a.extend(b) # 添加 b 的元素而不是 b 本身
>>> a
[45, 43624356, -3434, 1, 45, 23, 1, 111, 45, 56, 90]
```

##### 3. `sort()` ---- 将列表进行排序，前提是列表的元素可比较
```python
>>> a.sort()
>>> a
[-3434, 1, 1, 23, 45, 45, 45, 56, 90, 111, 43624356]
```


##### 3. `del` ---- 删除指定位置列表元素
```python
>>> del a[-1]
>>> a
[-3434, 1, 1, 23, 45, 45, 45, 56, 90, 111]
```

## 三. 栈 ---- 先进后出的数据结构

## 四. 队列 ---- 后进先出的数据结构

##### 1. `pop(i)` ---- 弹出第i项

##### 2. `attend(i)` ---- 将i加入列表的末尾
```python
>>> a = [1, 2, 3, 4, 5, 6]
>>> a
[1, 2, 3, 4, 5, 6]
>>> a.pop()
6
>>> a
[1, 2, 3, 4, 5,]
>>> a.append(34)
>>> a
[1, 2, 3, 4, 5, 34]
```
## 五. 元组 ---- 元组是由数个逗号分割的值组成，元组是不可变类型，这意味着你不能在元组内删除或添加或编辑任何值

##### 1. 元组的创建：
```python
>>> a = (123)
>>> a
123
>>> type(a)
<class 'int'>
>>> a = (123, )
>>> b = 321,
>>> a
(123,)
>>> b
(321,)
>>> type(a)
<class 'tuple'>
>>> type(b)
<class 'tuple'>
```

## 六. 字典 ---- 无序的键值对（key:value）集合，同一个字典内的key必须不相同。

##### 1. `del(key)` ---- 删除指定的键值对
```python
>>> data = {'kushal':'Fedora', 'kart_':'Debian', 'Jace':'Mac'}
>>> del data['kushal']
>>> data
{'kart_':'Debian', 'Jace':'Mac'}

```

##### 2. `in(key)` ---- 指定的key是否在该字典内
```python
>>> 'ShiYanLou' in data
False
>>> 'Jace' in data
True
```

##### 1. `dict()` ---- 从包含键值对的字典中创建元组
```python
>>> a = 123, 234
>>> a
(123, 234)
>>> b= 'aaa', 'bbb'
>>> b
('aaa', 'bbb')
>>> dict((a,b))
{123: 234, 'aaa': 'bbb'}
>>> dict(k1=1,k2='v2')
{'k2': 'v2', 'k1': 1}
```
##### 2. `items()` ---- 遍历字典
```python
>>> data
{'Kushal': 'Fedora', 'Jace': 'Mac', 'kart_': 'Debian', 'parthan': 'Ubuntu'}
>>> for x, y in data.items():
...     print("{} uses {}".format(x, y))
...
Kushal uses Fedora
Jace uses Mac
kart_ uses Debian
parthan uses Ubuntu
```
##### 3. `dict.setdefault(key, default)` ---- 判断字典中是否有改关键字，不存在则创建关键字
```python
>>> data = {}
>>> data.setdefault('names', []).append('Ruby')
>>> data
{'names': ['Ruby']}
>>> data.setdefault('names', []).append('Python')
>>> data
{'names': ['Ruby', 'Python']}
>>> data.setdefault('names', []).append('C')
>>> data
{'names': ['Ruby', 'Python', 'C']}
```
##### 4. `enumerate()` ---- 遍历字典并获得索引
```python
>>> for i, j in enumerate(['a', 'b', 'c']):
...     print(i, j)
...
0 a
1 b
2 c
```
##### 5. `zip(a,b)` ---- 同时遍历2个序列类型
```python

```