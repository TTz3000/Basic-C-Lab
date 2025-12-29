## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    int N, i ;
    int conutfizzbuzz = 0 ;
    int countfizz = 0 ;
    int countbuzz = 0 ;
    int otherconut = 0 ;
    
    if (scanf("%d" , &N ) != 1 ) {
        return 1 ; 
    }

    for( i = 1 ; i <= N ; i++ ) {
        if( i % 3 == 0 && i % 5 == 0 ) {
            conutfizzbuzz ++ ;
        } else if ( i % 3 == 0 && i % 5 != 0 ) {
            countfizz ++ ;
        } else if ( i % 3 != 0 && i % 5 == 0 ) {
            countbuzz ++ ;
        } else {
            otherconut ++ ;
        }
    }
    
    printf("Count FizzBuzz (by 15) : %d\n" , conutfizzbuzz ) ;
    printf("Count Fizz (by 3 only) : %d\n" , countfizz) ;
    printf("Count Buzz (by 5 only) : %d\n" , countbuzz) ;
    printf("Count Other: %d\n", otherconut ) ;
    return 0 ;
}
```

## TEST CASE
### Input
```c++
15
```
### Output
```c++
Count FizzBuzz (by 15) : 1
Count Fizz (by 3 only) : 4
Count Buzz (by 5 only) : 2
Count Other: 8
```




****
