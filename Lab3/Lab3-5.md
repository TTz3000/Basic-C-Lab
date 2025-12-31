## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

struct Order {
    int itemId;
    float unitPrice;
    int quantity;
};

int main() {
    int N, i;
    float grandTotal = 0;
    float Shiping_fee = 50 ;
    
    if (scanf("%d", &N) != 1) {
        return 1;
    }

    struct Order orders[N];
    
    for (i = 0; i < N; i++) {
        float itemTotal; 
        if (scanf("%d %f %d", &orders[i].itemId, &orders[i].unitPrice, &orders[i].quantity) != 3) {
            return 1;
        }
        
        itemTotal = (orders[i].unitPrice * orders[i].quantity) + Shiping_fee;
  
        if (itemTotal >= 500.0) {
            itemTotal *= 0.9 ;  
        } 
 
        grandTotal += itemTotal;
    }
    
    printf("Grand Total : %.2f \n" , grandTotal);
    return 0;
}
```

## TEST CASE
### Input
```c++
2
111
480
1
222
100
9
```
### Output
```c++
Grand Total : 1332.00 
```




****
