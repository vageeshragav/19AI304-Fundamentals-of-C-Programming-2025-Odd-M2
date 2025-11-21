
The program should display the average marks up to two decimal places and the corresponding grade. 

# Date : 
# Date : 21.11.2025
# Aim:
To build a C program that receives inputs for a student’s marks in three subjects, calculates the average, and determines the grade using nested if-else statements with safe floating-point comparisons.
# Algorithm:
@@ -56,15 +56,48 @@
### Step 11:
Stop
# Program:
```
#include <stdio.h>
int main() {
    float math, science, english, avg;
    printf("Enter marks in Math: ");
    scanf("%f", &math);
    printf("Enter marks in Science: ");
    scanf("%f", &science);
    printf("Enter marks in English: ");
    scanf("%f", &english);
    avg = (math + science + english) / 3.0;
    printf("\nAverage Marks: %.2f\n", avg);

    if (avg >= 90.0) {
        printf("Grade: A\n");
    } else {
        if (avg >= 75.0) {
            printf("Grade: B\n");
        } else {
            if (avg >= 50.0) {
                printf("Grade: C\n");
            } else {
                printf("Grade: F\n");
            }
        }
    }

    return 0;
}
```
# Output:

<img width="471" height="258" alt="image" src="https://github.com/user-attachments/assets/a02666ae-d931-4feb-abbd-b88cc782cc66" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:7
Develop a C program to display the multiplication table of a given number (15) up to 10.
# Date : 
# Date : 21.11.2025
# Aim:
To develop a C program that prints the multiplication table of the number 15 up to 10 using a for loop.
# Algorithm:
@@ -88,15 +121,30 @@ Thus, the program was implemented and executed successfully, and the required ou
Stop

# Program:
```
#include <stdio.h>
int main() {
    int num = 15;
    printf("Multiplication Table of %d\n", num);

    for (int i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", num, i, num * i);
    }
    return 0;
}
```
# Output:

<img width="445" height="399" alt="image" src="https://github.com/user-attachments/assets/362f4124-254e-4a3d-a75f-9e6140a5cf32" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:8
Develop a C program to check whether a given number is prime or not.
# Date : 
# Date : 21.11.2025
# Aim:
To develop a C program that determines whether an input number is a prime number using a while loop.
# Algorithm:
@@ -131,7 +179,33 @@ Thus, the program was implemented and executed successfully, and the required ou
### Step 7:   
Stop
# Program:
```
#include <stdio.h>
int main() {
    int num, i, isPrime = 1;
    printf("Enter a number: ");
    scanf("%d", &num);
    if (num < 2) {
        isPrime = 0;
    } else {
        for (i = 2; i * i <= num; i++) {
            if (num % i == 0) {
                isPrime = 0;
                break;
            }
        }
    }
    if (isPrime)
        printf("%d is a Prime Number\n", num);
    else
        printf("%d is Not a Prime Number\n", num);
    return 0;
}
```
# Output:

<img width="430" height="162" alt="image" src="https://github.com/user-attachments/assets/2ecf5c7f-79ed-4fe8-8d23-1e4059b9b4f7" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

@@ -147,7 +221,7 @@ Thus, the program was implemented and executed successfully, and the required ou
4   2  
54321
```
# Date : 
# Date : 21.11.2025
# Aim:
To build a C program that prints the required numeric pattern for a given value of n using nested loops.
# Algorithm:
@@ -179,7 +253,36 @@ Thus, the program was implemented and executed successfully, and the required ou
### Step 8:   
Stop
# Program:
```
#include <stdio.h>
int main() {
    int i, j;
    for (i = 1; i <= 5; i++) {
        printf("%d", i);
    }
    printf("\n");
    for (i = 2; i <= 4; i++) {
        for (j = 1; j <= 5; j++) {
            if (j == 1)
                printf("%d", i);
            else if (j == 5)
                printf("%d", 6 - i);
            else
                printf(" ");
        }
        printf("\n");
    }
    for (i = 5; i >= 1; i--) {
        printf("%d", i);
    }
    printf("\n");
    return 0;
}
```
# Output:

<img width="173" height="214" alt="image" src="https://github.com/user-attachments/assets/d5b74ea6-25ab-4b40-b97f-997869d05bac" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

@@ -232,6 +335,35 @@ Thus, the program was implemented and executed successfully, and the required ou
Decrease i by 1 and go back to Step 6.
### Step 8:
Stop
# Program :
```
#include <stdio.h>
int main() {
    int i, j;
    printf("0\n");
    for (i = 7; i >= 1; i--) {
        for (j = i; j <= 7; j++) {
            printf("%d ", j);
        }
        printf("0 ");
        for (j = 7; j >= i; j--) {
            printf("%d ", j);
        }
        printf("\n");
    }
    for (j = 0; j <= 7; j++)
        printf("%d ", j);
    printf("0 ");
    for (j = 7; j >= 0; j--)
        printf("%d ", j);
    printf("\n");
    return 0;
}
```
# Output :

<img width="437" height="336" alt="image" src="https://github.com/user-attachments/assets/502e191d-8454-4c5c-b9bd-32a16976c220" />

# Result:
Thus, the program was implemented and executed successfully, and the required output was obtained.
