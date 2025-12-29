## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    int termcode ;
    float investmentamount;
    float aprrate = 0.0 ;
    float totalinterest = 0.0 ;

    if(scanf("%d %f" , &termcode , &investmentamount) != 2 ) {
        return 1 ;
    }
    
    if(termcode == 1) {
        if (investmentamount < 5000) {
            aprrate = 0.03 ;
        } else if (investmentamount >= 5000) {
            aprrate = 0.04 ;
        }
    }else if(termcode == 2) {
        if (investmentamount < 10000) {
            aprrate = 0.05 ;
        } else if (investmentamount >= 10000) {
            aprrate = 0.065 ;
        }
    }else if(termcode == 3) {
        aprrate = 0.08 ;
    }

    if (termcode >= 1 && termcode <= 3) {
        totalinterest = investmentamount * aprrate ;
        printf("%.2f\n" , totalinterest);
    } else {
        printf("Invalid Term Code\n");
    }

    

    return 0 ;
}
```

## TEST CASE
### Input
```c++
2
12000
```
### Output
```c++
780.00
```




****
