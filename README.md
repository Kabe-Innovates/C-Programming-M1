# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    char firstChar, secondChar, thirdChar;

    scanf(" %c", &firstChar);
    scanf(" %c", &secondChar);
    scanf(" %c", &thirdChar);

    printf("%c %c %c\n", thirdChar, secondChar, firstChar);

    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/c086c866-27a1-4fee-8437-2e9b7940a4ff)

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.
<hr>

# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```c
#include <stdio.h>

int main() {
    int a;

    scanf("%d", &a);

    if (a > 0) {
        printf("Positive number\n");
    } else {
        printf("Not a positive number\n");
    }

    return 0;
}
```
# OUTPUT:

![image](https://github.com/user-attachments/assets/3e7391f7-b603-4170-9266-d8b93d260dff)

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
<hr> 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    int num1, denom1, num2, denom2;
    float fraction1, fraction2, minFraction;
    printf("Enter numerator and denominator for first fraction: ");
    scanf("%d %d", &num1, &denom1);
    printf("Enter numerator and denominator for second fraction: ");
    scanf("%d %d", &num2, &denom2);
    fraction1 = (float) num1 / denom1;
    fraction2 = (float) num2 / denom2;
    printf("Fraction 1: %d/%d = %.4f\n", num1, denom1, fraction1);
    printf("Fraction 2: %d/%d = %.4f\n", num2, denom2, fraction2);
    minFraction = (fraction1 < fraction2) ? fraction1 : fraction2;
    printf("Minimum fraction value: %.4f\n", minFraction);
    return 0;
}

```
## OUTPUT:

![image](https://github.com/user-attachments/assets/83645873-f780-4db7-b076-b59f3f05a09a)

## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.

<hr>


# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    int inputValue;

    scanf("%d", &inputValue);

    if (inputValue == 1) {
        printf("Input is equal to 1\n");
    } else {
        printf("Input is not equal to 1\n");
    }

    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/ff8f8130-31f1-43ab-b67c-cc4abac00010)

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully

<hr>

# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```c
#include <stdio.h>

int main() {
    int mark1, mark2, mark3;
    float total, percentage;

    scanf("%d", &mark1);
    scanf("%d", &mark2);
    scanf("%d", &mark3);

    total = mark1 + mark2 + mark3;
    percentage = total / 3;

    printf("%.2f\n", total);
    printf("%.2f\n", percentage);

    if (mark1 >= 40 && mark2 >= 40 && mark3 >= 40) {
        if (percentage >= 60) {
            printf("Division = First\n");
        } else if (percentage >= 48) {
            printf("Division = Second\n");
        } else if (percentage >= 36) {
            printf("Division = Pass\n");
        } else {
            printf("Division = Fail\n");
        }
    } else {
        printf("Division = Fail\n");
    }

    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/e5fff49a-7461-4973-af43-2aa90f6dbda3)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

