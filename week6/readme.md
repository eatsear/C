짝수의 합 -> 다른 방식으로!

```c
#include <stdio.h>

int main(void) {
   int n, sum;

   printf("정수를 입력하세요: ");
   scanf("%d", &n);

   if(n % 2 == 1) {
      sum = ((2 + (n-1))/2)*((n-1)/2); }
   else {
      sum = ((2 + n)/2)*(n/2); }

   printf("%d", sum);

   return 0;
}
```
