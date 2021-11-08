# EX1
NumClass.h
EX1
#ifndef NUMCLASS_H_INCLUDED
#define NUMCLASS_H_INCLUDED

/* will return if a number is Armstrong number
An Armstrong number is an n-digit number that is equal to the sum of the nth powers of its digits.
For Example: 407 = 43 + 03 + 73 = 64 + 0 + 343 = 407
*/
int isArmstrong(int)
/* will return if a number is a palindrome */
int isPalindrome(int)
/* will return if a number is prime*/
int isPrime(int)
/*Strong number is a special number whose sum of the factorial of digits is equal to the original
number. For Example: 145 is strong number
1! + 4! + 5! = 145
*/
int isStrong(int)

#endif // NUMCLASS_H_INCLUDED
=======
#include <stdio.h>
main
#include <stdlib.h>

int main()
{
    int number1 = 0, number2 = 0, i = 0, k = 0;
    scanf("%d", &number1);
    scanf("%d", &number2);
     if(number1 < number2)
     {
         i = number1;
         k = number2;
     }
     else
     {
        i = number2;
        k = number1;
     }
     for(i; i <= k; i++)
     {
         if(isPrime(i))
         {
             printf(i + " ");
         }
     }
     printf("",ln);
     for(i; i <= k; i++)
     {
         if(isArmstrong(i))
         {
             printf(i + " ");
         }
     }
     printf("",ln);
     for(i; i <= k; i++)
     {
         if(isStrong(i))
         {
             printf(i + " ");
         }
     }
     printf("",ln);
     for(i; i <= k; i++)
     {
         if(isPalindrome(i))
         {
             printf(i + " ");
         }
     }
    return 0;
}
=======
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
 basicClassification.c
main
