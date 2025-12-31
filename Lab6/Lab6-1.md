## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

void increase( int *number_plr ) ;

int main(){
    int data ;

    printf("Enter initial integer value : " );
    while (scanf("%d" , &data ) != 1 ) {
        return 1 ;
    }

    printf("\n|--- Pointer modification report ---|\n" ) ;
    printf("1. Value before function call : %d\n" , data ) ;
    increase( &data  ) ;
    printf("2. Value after function call : %d\n" , data ) ;

    return 0 ;
}

void increase( int *data ) {
    *data += 10 ;
}
```

## TEST CASE
### Input
```c++
Enter initial integer value : 60

```
### Output
```c++
|--- Pointer modification report ---|
1. Value before function call : 60
2. Value after function call : 70
```




****
