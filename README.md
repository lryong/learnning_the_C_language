####  C语言学习笔记

C的数据类型：
基本类型 int和float
枚举类型
void类型
派生类型：指针，数组，结构类型，共用体和函数体


%E: 表示输出双精度实数

不带初始化的定义：带有静态存储持续时间的变量会被隐式初始化为 NULL（所有字节的值都是 0），其他所有变量的初始值是未定义的。

extern关键字

C中的左值和右值

使用dfine定义常量，使用const也可以定义常量。如果define已经被定义好，局部变量里面不能再重新定义。


c的存储类：
auto 所有局部变量的默认存储类，只能修饰局部变量
register 定义再寄存器中
static 指示编译器在程序的生命周期内保持局部变量的存在。
extern  提供一个全局变量的引用


JVM内存的划分有五片：
1. 寄存器
2. 本地方法区
3. 方法区
4. 栈内存
5. 堆内存


c语言没有布尔类型变量

在声明变量的时候如果没有确切的地址可以赋值，可以为指针附一个NULL值。

C不支持在函数外部返回局部变量的地址，除非局部变量为static变量。

C数组允许定义可存储相同类型数据项的变量，结构体在C中用户可以自定义的可用的数据类型，可存储不同类型的数据项。

为了使用指向该结构的指针访问结构的成员，必须使用“->”运算符.


C 语言又提供了一种数据结构，称为"位域"或"位段"。所谓"位域"是把一个字节中的二进位划分为几个不同的区域，并说明每个区域的位数。


C语言中的共用体类似与Golang里面的interface
共用体占用的内存应足够存储共用体中最大的成员。

结构和联合的区别：
1. 结构和联合都是由多个不同的数据类型成员组成, 但在任何同一时刻, 联合转只存放了一个被选中的成员, 而结构的所有成员都存在。 
2. 对于联合的不同成员赋值, 将会对其它成员重写, 原来成员的值就不存在了, 而对于结构的不同成员赋值是互不影响的。 

typedef是由编译器执行解释的，#define是由预编译器进行处理的。

整数提升： int -> unsigned int -> long -> unsigned long -> long long -> unsigned long long -> float -> double -> long double 


void * 类型表示未确定类型的指针。C、C++ 规定 void * 类型可以通过类型转换强制转换为任何其它类型的指针。



