# EX1
EX1
#include <stdio.h>
#include <stdbool.h>

int isPalindrome(int num)
{
    int r = 0,sum=0,temp = 0;
    temp=num;
    while(num>0)
    {
       r=num%10;
       sum=(sum*10)+r;
       num=num/10;
    }
    if(temp==sum)
    {
        return 1;
    }
    else
    {
        return 0;
    }
}

int isArmstrong(int num)
{
    int r = 0,sum = 0,temp = 0;
    temp = num;
    while(num > 0)
    {
       r = num % 10;
       sum = sum +(r*r*r);
       num = num / 10;
    }
    if(temp == sum)
    {
        return 1;
    }
    else
    {
        return 0;
    }
}
