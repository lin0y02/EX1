# EX1
EX1
#include <stdio.h>
#include <stdbool.h>

int isPrime(int  num)
{
    int i = 0;
    if(num == 1 || num == 2)
    {
        return 1;
    }
    for(i = 2; i < num; i++)
    {
        if(num % i == 0)
        {
            return 0;
        }
    }
    return 1;
}

int isStrong(int num)
{
    int sum=0;
    int k=num;
    int r = 0;
    while(k!=0)
    {
        r=k%10;
        int f=fact(r);
        k=k/10;
        sum=sum+f;
    }
    if(sum==num)
    {
        return 1;
    }
    else
    {
        return 0;
    }
}
int fact(int r)
{
    int mul=1;
    for(int i=1;i<=r;i++)
    {
        mul=mul*i;
    }
    return mul;
}

