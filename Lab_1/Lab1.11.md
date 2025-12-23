## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int categoryCode ;
    float price_before_vat ;
    float totalBill = 0.0 ;
    float vatAmount = 0.0 ;

    if (scanf("%f %d" , &price_before_vat , &categoryCode) != 2 ) {
        return 1 ;
    }

    if ( categoryCode == 1 ) {
        vatAmount = 1.07 ;
        totalBill = price_before_vat * vatAmount ;
    } else if ( categoryCode == 2 ) {
        vatAmount = 0 ;
        totalBill = price_before_vat ;
    } else if ( categoryCode == 3 ) {
        vatAmount = 1.15 ;
        totalBill = price_before_vat * vatAmount ;
    } 
    
    if (categoryCode >= 1 && categoryCode <= 3) {
        vatAmount = totalBill - price_before_vat ;
        printf("VAT Amount : %.2f\n" , vatAmount) ;
        printf("Total Pric : %.2f\n" , totalBill) ;
    } else {
        printf("Invalid Category\n") ;
    }
    
    return 0 ;
}
```

## TEST CASE
### Input
```c++
500 3
```
### Output
```c++
VAT Amount : 75.00
Total Pric : 575.00
```

****
