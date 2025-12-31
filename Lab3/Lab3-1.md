## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

struct Product {
    char name[50] ;
    int productId ;
    float price ;
} ;

int main() {
    
    struct Product item ;
    
    if (scanf("%d %f %s" , &item.productId , &item.price , item.name ) != 3 ) {
        return 1 ;
    }

    printf("Id : %d Price: %.2f Name: %s" , item.productId , item.price , item.name ) ; 
    return 0 ;
}
```

## TEST CASE
### Input
```c++
480
9500.65
TT
```
### Output
```c++
Id : 480 Price: 9500.65 Name: TT
```




****
