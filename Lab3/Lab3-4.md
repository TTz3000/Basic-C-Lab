## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

struct Student {
    char name[50] ;
    int studentId ;
    float score ;
} ;

int main() {
    int N , i ;
    int Passcount = 0 , Failcount = 0 ;

    if (scanf("%d" , &N ) != 1 ) {
        return 1 ;
    }
    
    struct Student students[N] ;
    
    for ( i = 0 ; i < N ; i++ ) {
        
        if (scanf("%d %f %s" , &students[i].studentId , &students[i].score , students[i].name ) != 3 ) {
            return 1 ;
        }
    }

    for ( i = 0 ; i < N ; i++ ) {   
        if ( students[i].score >= 60 ) {
            Passcount++ ;
        } else {
            Failcount++ ;
        }
    }
    
    printf("Pass Count : %d \n" , Passcount ) ;
    printf("Fail Count : %d " , Failcount ) ;

    return 0 ;
}
```

## TEST CASE
### Input
```c++
2
111
96
AAA
555
58
BBB
```
### Output
```c++
Pass Count : 1 
Fail Count : 1
```




****
