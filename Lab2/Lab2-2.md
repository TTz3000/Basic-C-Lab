## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    int N , i ,quanlity ;
    float uniprice , itemcost , grandtotal = 0.0 ;

    if(scanf("%d" , &N) != 1 ) {
        return 1 ;
    }

    for (int i = 0; i < N; i++) {
        itemcost = 0 ;
        scanf("%f %d" , &uniprice , &quanlity );
        if (uniprice >= 1000) {
            uniprice = uniprice * 0.9 ;
            itemcost = uniprice * quanlity ;
        } else {
            itemcost = uniprice * quanlity ;
        }
        grandtotal += itemcost ;
    }

    
    printf("Grand Total : %.2f\n" , grandtotal);
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
2000
1
500
2
Grand Total : 2800.00
```




****
