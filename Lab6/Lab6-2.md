## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

void swap_value(int *i, int *j) ;

int main() {
    int n1 , n2 ;
   
    printf("Enter value for Num1 : " );
    if (scanf("%d" , &n1 ) != 1 ) {
        return 1 ;
    }
    printf("Enter value for Num2 : " );
    if (scanf("%d" , &n2 ) != 1 ) {
        return 1 ;
    }
    
    printf("\n|--- Swapping Report! ---|\n" ) ;
    printf("Before swap - num1 : %d | num2 : %d\n" , n1 , n2 ) ;

    swap_value( &n1 , &n2 ) ;
    
    printf( "After swap - num1 : %d | num2 : %d " , n1 , n2 ) ;
    
    return 0 ;
}

void swap_value(int *i, int *j){
    *i = *i + *j ;
    *j = *i - *j ;
    *i = *i - *j ; 
}
```

## TEST CASE
### Input
```c++
Enter value for Num1 : 80
Enter value for Num2 : 60

```
### Output
```c++
|--- Swapping Report! ---|
Before swap - num1 : 80 | num2 : 60
After swap - num1 : 60 | num2 : 80
```




****
