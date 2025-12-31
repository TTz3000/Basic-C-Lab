## Computer Programming for Computer Engineer 

# CODE
```c++
#include <stdio.h>

struct empolyee{
    int id ;
    int gross_salary ;
    int bonus ;
    int total_income ;
} ;

int calculate_net_salary( int total_income ) ;

int main () {
    struct empolyee emp ;
    int net_salary = 0 ;

    printf("Enter Employee ID : " ) ;
    scanf( "%d" , &emp.id ) ;

    printf("Enter gross Salary : " ) ;
    scanf( "%d" , &emp.gross_salary ) ;

    printf("Enter Bonus : " ) ;
    scanf( "%d" , &emp.bonus ) ;

    emp.total_income = emp.gross_salary + emp.bonus ;
    net_salary = calculate_net_salary( emp.total_income ) ;

    printf( "\n|--- EMPLOYEE SALARY REPORT ---|\n" ) ;
    printf( "ID : %d\n" , emp.id ) ;
    printf( "Gross Salary : %d\n" , emp.gross_salary ) ;
    printf( "Bonus : %d\n" , emp.bonus ) ;
    printf( "Total Income : %d\n" , emp.total_income ) ;
    printf( "Net Salary : %d" , net_salary ) ;

    return 0 ;
}

int calculate_net_salary( int total_income ) {
    int tax = 0 ;
    int totalIC = 0 ;
    if( total_income > 30000 ){
        tax = total_income * 0.1 ;
    }else if (total_income <= 30000 ) {
        tax = total_income * 0.05 ;
    }
    totalIC = total_income - tax ;
    return totalIC ;
}
```

## TEST CASE
### Input
```c++
Enter Employee ID : 1412
Enter gross Salary : 50000
Enter Bonus : 2500
```
### Output
```c++
|--- EMPLOYEE SALARY REPORT ---|
ID : 1412
Gross Salary : 50000
Bonus : 2500
Total Income : 52500
Net Salary : 47250
```




****
