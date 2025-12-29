## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    float principal , monthlyPayment , interest ;
    int monthcount = 0 ;
    const float Interest_rate = 0.01 ;
    const float Penalty = 10.0 ;

    if(scanf("%f %f" , &principal , &monthlyPayment) != 2 ) {
        return 1 ;
    }


    while (monthcount < 10) {
        if (principal <= 0) {
            break;
        } else {
            interest = principal * Interest_rate ;
            principal = principal + interest ;
            if (monthlyPayment < interest) {
                principal = principal + 10 ;
            }
            principal = principal - monthlyPayment ;
            printf("Month %d : Remaining %.2f\n", ++monthcount , principal);
        }    
    }
    
    if (principal > 0) {
        printf("Loan settled in 10+ months. \n");
    } else {
        printf("Loan settled in %d months. \n" , monthcount);
    }
    
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
100
50
```
### Output
```c++
Month 1 : Remaining 51.00
Month 2 : Remaining 1.51
Month 3 : Remaining -48.47
Loan settled in 3 months.
```




****
