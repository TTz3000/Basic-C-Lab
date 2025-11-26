## Computer Programming for Computer Engineer - Lab 1.2

# CODE
```c++
#include <stdio.h>

int main() {
    int score ;

    if (scanf("%d", &score) != 1 ) {
        return 1 ;
    }

    if ( score >= 80 ) {
        printf("Grade A");
    }else if ( score >= 70 ) {
        printf("Grade B");
    }else if ( score >= 60 ) {
        printf("Grade C");
    }else if ( score >= 50 ) {
        printf("Grade D");
    }else if ( score < 50 ) {
        printf("Grade F");
    }

    return 0 ;
}
```

## TEST CASE
### Input
```c++
35
```
### Output
```c++
Grade F
```




****
