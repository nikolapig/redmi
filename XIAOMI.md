#2021/10/7 

3.1 顺序栈实现

#define MaxSize 50              //定义栈中元素的最大个数
typedef struct{
    Elemtype data[MaxSize];     //存放栈中的元素
    int top;                    //栈顶指针
}SqStack;

3.2 顺序栈的基本操作
1.InitSta    