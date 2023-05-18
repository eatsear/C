```c
#include <stdio.h>

int main(void) {
  int s, e;
  while(1) {
    printf("다음 조건에 만족하는 숫자 두 개를 입력하시오.\n");
    printf("{N| N는 정수, 2<=N<=9}\n");
    scanf("%d %d", &s, &e);
    if(2>s || 2>e || s>9 || e>9) {
      printf("INPUT ERROR!\n");
    } else {break;}
  }

  if(s>e) {
      for(int i=1; i<=9; i++) {
        for(int j=s; j>=e; j--) {
          printf("%d * %d = ", j, i);
          if(j*i<10) {printf(" %d", j*i);}
          else {printf("%d", j*i);}
          if(j!=e) {printf("   ");}
          else {printf("\n");}
        }
      }
    }
  else {
      for(int i=1; i<=9; i++) {
        for(int j=s; j<=e; j++) {
          printf("%d * %d = ", j, i);
          if(j*i<10) {printf(" %d", j*i);}
          else {printf("%d", j*i);}
          if(j!=e) {printf("   ");}
          else {printf("\n");}
        }
      }
    }

return 0;
}
```
