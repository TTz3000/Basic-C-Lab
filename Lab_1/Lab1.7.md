## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int customertype;
    float consumption_kwh;
    float totalbill = 0.0;

    if (scanf("%d %f" , &customertype , &consumption_kwh ) != 2 ) {
        return 1 ;
    }

    if ( customertype == 1 ) {
        if ( consumption_kwh > 100 ) {
            totalbill = consumption_kwh * 4 ;
        } else if ( consumption_kwh >= 0 ) {
            totalbill = consumption_kwh * 3 ;
        }
    } else if ( customertype == 2 ) {
        if ( consumption_kwh > 500 ) {
            totalbill = consumption_kwh * 6.5 ;
        } else if ( consumption_kwh >= 0 ) {
            totalbill = consumption_kwh * 5 ;
        }
    } else {
        printf(" Invalid Customer ") ;
        return 1 ;
    }

    if ( totalbill > 0.0 || customertype == 3 ) {
        printf("%0.2f" , totalbill ) ;
    }
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
1 50
```
### Output
```c++
150.00
```

****
