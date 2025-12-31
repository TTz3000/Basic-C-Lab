## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int main() {
    int N , i ;
    int Passscore = 0 , Failscore = 0 ;

    if( scanf("%d" , &N ) != 1 ) {
        return 1 ;
    } 

    int score[N] ;

    for ( i = 0 ; i < N ; i ++ ) {

        if (scanf( "%d" , &score[i] ) != 1 ){
            return 1 ;
        }

        if (score[i] >= 50 ) {
            Passscore += score[i] ;
        }else {
            Failscore++ ;
        }
    }

    printf("Passing Score Sum : %d \n" , Passscore ) ;
    printf("Failing Students Count : %d \n" , Failscore ) ;

    return 0 ;
}
```

## TEST CASE
### Input
```c++
8
50
40
90
80
40
60
70
80
```
### Output
```c++
Passing Score Sum : 430 
Failing Students Count : 2
```




****
