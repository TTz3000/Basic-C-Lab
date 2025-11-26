## Computer Programming for Computer Engineer - Lab 1.2

# CODE
```c++
#include <stdio.h>

int main() {
    int row, i ;

    scanf("%d", &row);
    if ( row < 1 ) {
        printf("Error");
        return 0;
    }

    for (int i = 0; i < row; i++)
    {
        printf("Hello Loop!\n");
    }
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
5
```
### Output
```c++
Hello Loop!
Hello Loop!
Hello Loop!
Hello Loop!
Hello Loop!
```




****
