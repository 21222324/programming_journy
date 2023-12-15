```c
#include <stdio.h>
// a quick example of using recursive functions
int fact(int a);
int main() {
  int x = 0;
  printf("enter a number: ");
  scanf("%d", &x);
  int result = fact(x);

  printf("%d ", result);

  return 0;
}
```

int fact(int a) {
  if (a == 1) {
    return 1;
  } else if (a == 0)
    return 0;

  else
    return fact(a - 1) + fact(a - 2);
}
