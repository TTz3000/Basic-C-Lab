## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int number ;

    do {
        printf("Enter a number (1-10) : ") ;
        if (scanf("%d", &number) != 1 ) {
            break;
        }

        if ( number < 1 || number > 10 ){
            printf("\nError : Value must be 1-10.\n");
        }

    } while ( number < 1 || number > 10 ) ;

    printf( "Input accepted : %d\n", number ) ;
    return 0 ;
}
```

## TEST CASE
### Input
```c++

```
### Output
```c++
Enter a number (1-10) : 15

Error : Value must be 1-10.
Enter a number (1-10) : -15

Error : Value must be 1-10.
Enter a number (1-10) : 6
Input accepted : 6
```

****
