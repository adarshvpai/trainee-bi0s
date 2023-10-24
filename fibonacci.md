#include <stdio.h>\
void Fibonacci(int n, int x) \
{\
    long a=0,b=1;\
    long c;\
    int i;\
    for (i=2;i<=n;i++) \
    {\
        c=a+b;\
        a=b;\
        b=c;\
    }\
    for (i=1;i<=x;i++)\ 
    {\
        printf("%ld ", b);\
        c=a+b;\
        a=b;\
        b=c;\
    }\
}\
int main()\ 
{\
    int n,x;\
    printf("Enter the value of n:");\
    scanf("%d",&n);\
    printf("Enter the number of Fibonacci numbers to print x:");\
    scanf("%d",&x);\
    if (n<0 || x<=0)\ 
    {\
        printf("Invalid input.");\
    } \
    else\ 
    {\
        Fibonacci(n,x);\
    }\
    return 0;\
}\
