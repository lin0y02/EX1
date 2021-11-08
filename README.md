# EX1
EX1
#include <stdio.h>
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
