#include <stdio.h>

long long factorial (int n){
       long long fact = 1;
        if (n < 0){
            return -1;
        }
   for (int i =1; i <=n; i++){
        fact *=i;
   }

   return fact;
   }

   int main() {
       int num;
       printf("Enter a number:");
       scanf("%d", &num);
       long long result = factorial(num);

       if (result == -1){
           printf("factorial is not defined for negative numbers.\n");
       }
       else {
            printf("factorial of %dis %lld\n", num, result);

       }
       return 0;
}