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
    int N, i ;
    
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
        printf("Id : %d Name : %s Score : %.2f\n" , students[i].studentId , students[i].name , students[i].score  ) ;
    }

    return 0 ;
}
```

## TEST CASE
### Input
```c++
3
67 
90
TT
69
86 
Pooh 
56
78
Yu
```
### Output
```c++
Id : 67 Name : TT Score : 90.00
Id : 69 Name : Pooh Score : 86.00
Id : 56 Name : Yu Score : 78.00
```




****
