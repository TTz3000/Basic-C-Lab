## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int planCode ;
    float dataUsage_GB ;
    float totalBill = 0.0 ;

    if (scanf("%d %f" , &planCode , &dataUsage_GB) != 2 ) {
        return 1;
    }

    switch (planCode)
    {
    case 1 :
        if ( dataUsage_GB <= 10 ) {
            totalBill = 299 ;
        } else if ( dataUsage_GB > 10 ) {
            totalBill = 299 + 10*(dataUsage_GB - 10);
        }
        break;
    case 2 :
        if ( dataUsage_GB <= 20 ) {
            totalBill = 599 ;
        } else if ( dataUsage_GB > 20 ) {
            totalBill = 599 + 50  + 5*(dataUsage_GB - 20);
        }
        break;
    default:
        break;
    }

    if ( planCode == 1 || planCode == 2 ) {
        printf("%.2f\n" , totalBill ) ;
    } else {
        printf("Invalid Plan Code\n") ;
    }
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
2 15
```
### Output
```c++
599.00
```

****
