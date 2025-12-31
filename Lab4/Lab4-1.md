## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    int N , i ;

    if( scanf("%d" , &N ) != 1 ) {
        return 1 ;
    } 

    int stuscores[N] ;

    for ( i = 0 ; i < N ; i ++ ) {
        if (scanf("%d" , &stuscores[i] ) != 1 ) {
            return 1 ;
        }
    }

    for ( i = N - 1 ; i >= 0 ; i -- ) {
        printf("%d\n" , stuscores[i] ) ;
    }
    return 0 ;
}
```

## TEST CASE
### Input
```c++
5
10
20
30
40
50
```
### Output
```c++
50
40
30
20
10
```




****
