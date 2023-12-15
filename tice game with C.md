## tice game
```c
#include<stdio.h>
#include<stdlib.h>
#include<time.h>

int main(void){

   unsigned int p1,p2;

    srand(time(NULL)); 

    p1= 1 + (rand() %12);

    p2= 1 + (rand() %12); 

     if(p2>p1) 

        printf("p1 role:%d, p2 role:%d => p2 win",p1,p2);

    else if(p1>p2) 

        printf("p1 role:%d, p2 role:%d => p1 win",p1,p2);

    else 

        printf("p1 role:%d, p2 role:%d => draw",p1,p2);
      
return 0;
 }
