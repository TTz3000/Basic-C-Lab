## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int clearancelevel , age , isActive;

    if (scanf("%d %d %d" , &clearancelevel , &age , &isActive) != 3) {
        return 1 ;
    }

    if (clearancelevel == 3 && isActive == 1 ) {
        printf("Access Granted");
    } else if (clearancelevel == 2 && age >=25 && isActive == 1) {
        printf("Access Granted");
    } else {
        printf("Access Denied");
    }
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
3 30 1
```
### Output
```c++
Access Granted
```

****
