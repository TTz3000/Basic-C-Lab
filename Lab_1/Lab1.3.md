## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int i1, i2, opcode, total;

    printf("Input : Num1, Num2, OpertionCode\n");
    if(scanf("%d %d %d", &i1, &i2, &opcode) != 3) {
        return 1 ;
    }

    if(opcode == 1){
        total = i1 + i2 ;
    }else if (opcode == 2) {
        total = i1 - i2 ;
    }else if (opcode == 3) {
        total = i1 * i2 ;
    }else if (opcode == 4) {
        total = i1 / i2 ;
    }else{
        printf("Invalid Operation!");
    }

    printf("\n%d", total);
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
Input : Num1, Num2, OpertionCode
10 4 3
```
### Output
```c++
40
```

****
