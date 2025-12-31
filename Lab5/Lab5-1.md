## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

int calculate_area( int length , int width ) ;

int main () {
    int input_a , input_l ,input_w ;

    printf( "Enter length and width : " ) ;
    if(scanf( "%d %d" , &input_l , &input_w ) !=2 ) {
        return 1 ;
    }

    input_a = calculate_area( input_l , input_w ) ;
    printf( "\n|----RECTANGLE AREA REPORT----|\n" ) ;
    printf( "Length : %d\n" , input_l ) ;
    printf( "Width : %d\n" , input_w ) ;
    printf( "Calculated Area : %d\n" , input_a ) ;

    return 0 ;
}

int calculate_area( int length , int width ) {
    int area ;
    area = length * width ;
    return area ;
}
```

## TEST CASE
### Input
```c++
Enter length and width : 5 4 
```
### Output
```c++
|----RECTANGLE AREA REPORT----|
Length : 5
Width : 4
Calculated Area : 20
```




****
