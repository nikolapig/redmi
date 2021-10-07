#2021/10/7 

3.1 顺序栈实现
<br>
`#define MaxSize 50`          //定义栈中元素的最大个数<br>
`typedef struct{`<br>
    `Elemtype data[MaxSize];`     //存放栈中的元素<br>
    `int top;`                   //栈顶指针<br>
`}SqStack;`<br>
<br>
栈顶指针：S.top，初始设置S.top=-1；                 
栈顶元素：S.data[S.top].<br>
进栈操作：栈不满时，栈顶指针先加1，再加数据存入栈顶。<br>
出栈操作：栈非空时，先取出栈顶的元素，再将栈顶的指针减1。<br>
栈空条件：S.top==-1；                    
栈满条件：S.top==MaxSize-1;                      
栈长：S.top+1;            

3.2 顺序栈的基本操作<br>
1.`void InitStack(SqDtack S){<br>
    S.top=-1;<br>
}`