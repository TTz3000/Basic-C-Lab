## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int dayCode, hour;

    if (scanf("%d %d" , &dayCode, &hour) != 2 ) {
        return 1 ;
    }

    if ( dayCode <= 5  ) {
        if ( hour >= 8 && hour <= 17 ) {
            printf("System Running (Workday)");
        } else {
            printf("System Idle (Off-hours)");
        }
        
    } else if ( dayCode <= 7 ) {
        printf("Weekend Relex Mode");
    } else {
        printf("Invalid Day Code");
    }
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
3 17
```
### Output
```c++
System Running (Workday)
```

****
