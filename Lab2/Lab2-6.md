## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    int N_months , month , successconut = 0 ;
    float dailyDeposit , monthlytotal ;

    if (scanf("%d" , &N_months) != 1 ) {
        return 1 ;
    }

    for (month = 1 ; month <= N_months ; month++) {
        monthlytotal = 0.0 ;

        if (scanf("%f" , &dailyDeposit) != 1 ) {
            break ;
        }

        while (dailyDeposit != 0.00) {
            monthlytotal = monthlytotal + dailyDeposit ;
            if (scanf(" %f" , &dailyDeposit) != 1 ) {
                break ;
            } 
        }
        
        if (monthlytotal > 500) {
            successconut++ ;
        }
        
        printf("Month %d Total : %.2f\n" , month , monthlytotal);  
    }

    printf("Success Count : %d\n" , successconut ) ;
    return 0 ;
}
```

## TEST CASE
### Input
```c++

```
### Output
```c++
2
600
20
0
Month 1 Total : 620.00
30
48
0
Month 2 Total : 78.00
Success Count : 1
```




****
