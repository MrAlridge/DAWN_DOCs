# 关于指针上机中出现的问题
========================
## 1.指向字符串的指针
```C
    #include<stdio.h>

    int main()
    {  
        char *string = "I Love China!";
        printf("%s\n",string);
        getchar();
        return 0;
    }
```
如上代码,在实际上机时错敲成下面这段:
```C
char *string[] = "I Love China!";       //这是错的
```
这样定义的string数组是一个 ***指向字符型变量*** 的*指针数组*.