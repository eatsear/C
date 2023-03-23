# 4주차 C언어 수업

## 4_01.c
```c
#define _CRT_NO_SECURE_WARNINGS
#include <stdio.h>

int main(void) {
    int a, b, c, d, e;

    printf("물건 값을 입력하시오: ");
    scanf("%d", &a);

    printf("투입한 금액을 입력하시오: ");
    scanf("%d", &b);

    printf("거스름돈은 다음과 같습니다");

    c = b - a;
    d = c / 1000;
    printf("천원권: %d장\n", d);

    e = c % 1000;
    d = e / 500;
    printf("오백원권: %d장\n", d);

    e = c % 500;
    d = e / 100;
    printf("백원권: %d장", d);

    return 0;
}
```
