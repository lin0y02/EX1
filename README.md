# EX1
EX1
#include <stdio.h>
#include<math.h>
#include <stdbool.h>


int rev(int num, int temp)
{
    if (num == 0)
    {
         return temp;
    }
    temp = (temp * 10) + (num % 10);
    return rev(num / 10, temp);
}


int isPolindrome (int num)
{
    int temp = num;
    temp = rev(num, 0);

    if (temp == num)
    {
        printf("%d is palindrome\n", num);
    }
    else
    {
        printf("%d is not palindrome\n", num);
    }
}


int check_ArmstrongNumber(int num)
{
    if(num>0)
    {
        return (pow(num%10,3) + check_ArmstrongNumber(num/10));
    }
}

int isArmstrongg(int num){
   if(check_ArmstrongNumber(num)==num)
   {
       printf("%d is an Armstrong\n", num);
       return true;
   }
   else
   {
       printf("%d is not an Armstrong\n", num);
       return false;
   }
}
