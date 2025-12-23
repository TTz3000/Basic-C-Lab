## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int zoneCode ;
    float weigth_kg ;
    float totalCost = 0.0 ;

    if (scanf("%d %f" , &zoneCode , &weigth_kg) != 2 ) {
        return 1 ;
    }

    switch (zoneCode)
    {
    case 1 :
        if ( weigth_kg <= 5 ) {
            totalCost = 50 ;
        } else if ( weigth_kg > 5 ) {
            totalCost = 80 ;
        }  
        break;
    case 2:
        if ( weigth_kg <= 10 ) {
            totalCost = 150 ;
        } else if ( weigth_kg > 10 ) {
            totalCost = 250 ;
        }
        break;
    case 3:
        totalCost = 500 ;
        break;
    default:
        printf("Invalid Zone Code");
        break;
    }

    if (totalCost > 0.0 || zoneCode > 3 || zoneCode < 1) {
        printf("%.2f\n" , totalCost ) ;
    }

    return 0 ;
}
```

## TEST CASE
### Input
```c++
1 2.6
```
### Output
```c++
50.00
```

****
