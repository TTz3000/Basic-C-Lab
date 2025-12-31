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
    float Average_s = 0.00 ; 

    if (scanf("%d" , &N ) != 1 ) {
        return 1 ;
    }

    
    struct Student students[N] ;
    
    
    for ( i = 0 ; i < N ; i++ ) {
        
        if (scanf("%d %f %s" , &students[i].studentId , &students[i].score , students[i].name ) != 3 ) {
            return 1 ;
        }
        Average_s = Average_s + students[i].score ;
    }
    
    Average_s = Average_s / N ;
    printf("Average Score : %.2f " , Average_s ) ;
    

    return 0 ;
}
```

## TEST CASE
### Input
```c++
2
888
50
AA
777
100
DD
```
### Output
```c++

Average Score : 75.00 
```




****
