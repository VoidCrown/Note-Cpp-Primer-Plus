# Chapter 2

## 2.1 

```c++
//myfirst.cpp
#include<iostream>
int main()
{
    using namespace std;
    cout << "Hello world!";
    cout << endl;
    return 0;
}
```

```int main()``` 

- C++： ()与void等价
- C: () 对是否接受参数保持沉默

### 注释：

- C++：```//```
- C：```/* */```

### 头文件名

- C++新式：iostream, namespace std
- C转换：cmath, namespace std(可以用不是C的特性)
- C++旧：math.h
- C传统：iostream.h

### C++源代码格式化

1. 标记和空白

   - 标记(token)：一行代码中不可分割的元素

   - 空白(white space)：空格，制表符和回车

2. C++风格
   - 每行语句占一行
   - 每个函数都有一个开始花括号和一个结束花括号，这两个花括号各占一行
   - 函数中的语句都相对于花括号进行缩进
   - 于函数名称相关的圆括号周围没有空白

## 2.2 C++语句

```c++
//2.2 carrot.cpp
#include<iostream>

int main()
{
    using namespace std;
    
    int carrots;
    carrots = 25;
    
    cout << "I have " << carrots << " carrots." << endl;
    carrots = carrots - 1;
    cout << "Now ,I have " << carrots << " carrots." << endl;
    
    return 0;
}
```

### 声明语句和变量

要将信息存储在计算机中，必须指出信息的存储位置和所需的内存空间。

C++中，使用声明语句来指出存储类型并提供位置标签

`int carrots` 提供两条信息：

- 需要的内存
- 给存储单元指定名称

定义声明(defining declaration)语句：编译器为变量分配内存空间

引用声明(reference declaration)语句：使用在其他地方定义的变量

[***<u>C++尽可能在首次使用变量前声明</u>***]()

### 函数

被调用函数(called function)：被调用的函数

调用函数(calling functio)： 包含函数调用的函数

***<u>C++程序应该为程序中使用的每个函数提供原型</u>***

e.g.`double sqrt(double);`

提供原型的两种方法：

- 在源代码中输入函数原型
- 包含带有函数原型的头文件

函数的特性：

- 有函数头和函数体
- 接受参数
- 返回值
- 需要一个原型