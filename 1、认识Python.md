# Python

一. 函数：
1. `print()`----- 多行打印，3个单引号。
```python
print('''
        我去买几个橘子，
        你站在此地不要动
    ''');
```
2. `input()`----- 让用户输入某个内容并接收它
```python
    age = inpur('My age is:');
```

3. `format()`  
        - 第一种：占位符 ---  
```python
    print('你叫{}，今年{}岁了'.format(name,age));
```
        - 第二种：数字格式化 ---  
            - {:.0f}   不带小数
   			- {:.2f}   2位小数
            - {:.3f}   3位小数
4. `divmod(num1,num2)`  
   - 第一个值为num1和num2相除得到的值；
   - 第二个值为num1和num2求余得到的值；

二. 数据类型：
int，float，字符串，布尔，None，列表，元组，字典，集合等。

三.  运算符：
1. 逻辑运算符：
   1. 与、或、非 --- and/or/not  
   ```python
      #其中not具有最高运算级别，and次之，or最低
      A and not B or C === (A and (not B))or C
    ```

注意：
1. 任意一个操作是浮点数，结果就是浮点数；
2. 除法结果除不尽时，结果将会是小数。
![运算符](./assets/jc.png)