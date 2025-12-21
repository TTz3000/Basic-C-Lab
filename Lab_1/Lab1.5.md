## Computer Programming for Computer Engineer

# CODE
```c++
#include <stdio.h>

int main() {
    int number;
    int evensum = 0 ;
    int oddsum = 0 ;

    if ( scanf(" %d", &number ) != 1 ) {
        return 1 ;
    }

    while ( number != 0 ) { 
        if (number % 2 == 0) {
            evensum += number ;
        } else {
            oddsum += number ;  
        }
        
        if (scanf("%d", &number) != 1) {
            break;
        }  
        if (number == 0) {
            break;
        }
    }

    printf("Even sum : %d\n", evensum ) ;
    printf("Odd sum : %d\n", oddsum ) ;
    return 0 ;
}
```

## TEST CASE
### Input
```c++
5
7
2
8
0
```
### Output
```c++
Even sum : 10
Odd sum : 12
```

****
