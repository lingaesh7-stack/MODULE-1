# NAME : LINGAESHWAR K

# MODULE-1-
Module 1 respository for lab

# C Programming Practice Programs

# 1.Program: Display Character from ASCII Value

**Aim:**

To write a C program that reads an integer value and displays its corresponding ASCII character.



**Algorithm:**  

1. Start the program.  
2. Declare an integer variable num.  
3. Read the integer input from the user using scanf().  
4. Use the printf() function to display the corresponding ASCII character of the entered number using %c format specifier.  
5. End the program.


**Source Code:**

```c
#include <stdio.h>
int main()
{
    int num;
    scanf("%d", &num);
    printf("Character of ASCII Value %d is %c", num, num);
    return 0;
}

# output

<img width="780" height="199" alt="image" src="https://github.com/user-attachments/assets/ed1ffff5-9456-476c-b00b-87bcc8810f8a" />



**Result:**
The program successfully prints the character corresponding to the given ASCII value.
---

# 2.Program: Check if Number is Equal to 000

**Aim:**  
To write a C program that checks whether the input number is equal to 000.



*Algorithm:*  
1. Start the program.  
2. Declare an integer variable num.  
3. Read an integer input from the user using scanf().  
4. Use an if statement to compare the number with 000.  
   - If equal → print "Number is equal to 000".  
   - Otherwise → print "Number is NOT equal to 000".  
5. End the program.



*Source Code:*
c
#include <stdio.h>
int main()
{
    int num;
    scanf("%d", &num);
    if(num == 000)
        printf("Number is equal to 000");
    else
        printf("Number is NOT equal to 000");
    return 0;
}

*output*

<img width="698" height="250" alt="image" src="https://github.com/user-attachments/assets/5d7c460d-0b7b-4d8b-8d71-7134dd76bf13" />



*Result:*
The program correctly checks whether the entered number is 000 and displays the appropriate message.

---
3.# Program: Simple and Compound Interest Calculation

*Aim:*  
To write a C program that calculates both the Simple Interest (SI) and Compound Interest (CI) for a given principal, rate of interest, and time period.


*Algorithm:*  
1. Start the program.  
2. Declare float variables principle, Year, rate, SI, and CI.  
3. Read input values for principal, time (in years), and rate of interest using scanf().  
4. Calculate *Simple Interest* using the formula:  
(Use pow() from math.h for exponentiation)  
6. Print the calculated SI and CI using printf().  
7. End the program.



*Source Code:*
c
#include <stdio.h>
#include <math.h>

int main()
{
 float principle, Year, rate, CI, SI;
 
 scanf("%f", &principle);
 scanf("%f", &Year);
 scanf("%f", &rate);
 
 SI = (principle * Year * rate) / 100;
 printf("Simple Interest = %.2f \n", SI);
 
 CI = principle * (pow((1 + rate / 100), Year));
 printf("Compound Interest = %.2f \n", CI);
 
 return 0;
}

*output*

<img width="736" height="140" alt="image" src="https://github.com/user-attachments/assets/8e45d22b-70b2-4fbb-af6a-c0ce5f74caa6" />


*Result:*

The program correctly calculates and displays the Simple Interest and Compound Interest for the given inputs.
---
4.# Program: Arithmetic Operations Using Switch Statement

*Aim:*  
To write a C program that performs basic arithmetic operations (+ and -) on two numbers using a switch statement.



*Algorithm:*  
1. Start the program.  
2. Declare integer variables num1 and num2 for storing numbers, and a character variable op for the operator.  
3. Read input values for num1, op, and num2 using scanf().  
4. Use a switch statement to evaluate the operator:  
   - Case '+' → Add num1 and num2 and print the result.  
   - Case '-' → Subtract num2 from num1 and print the result.  
   - Default → Print "Invalid Input" if the operator is not recognized.  
5. End the program.



*Source Code:*
c
#include <stdio.h>
int main()
{
    int num1, num2;
    char op;
    scanf("%d %c %d", &num1, &op, &num2);
    
    switch (op) {
        case '+' :
            printf("Result = %d", num1 + num2);
            break;
        case '-' :
            printf("Result = %d", num1 - num2);
            break;
        default :
            printf("Invalid Input");
    }
    return 0;
}

*output*

<img width="459" height="294" alt="image" src="https://github.com/user-attachments/assets/36dc10bd-ebe5-47ae-970e-c0e5b78a1677" />


*Result:*
The program successfully performs addition or subtraction based on the operator entered by the user and displays the correct result.
---

5.# Program: Grade Evaluation Based on Marks

*Aim:*  
To write a C program that reads a student's marks and prints the corresponding grade message.


*Algorithm:*  
1. Start the program.  
2. Declare an integer variable marks.  
3. Read the marks from the user using scanf().  
4. Use if-else if-else statements to determine the grade:  
   - Marks ≥ 70 → "VERY GOOD"  
   - 60 ≤ Marks < 70 → "GOOD"  
   - 50 ≤ Marks < 60 → "ABOVE AVERAGE"  
   - 40 ≤ Marks < 50 → "AVERAGE"  
   - Marks < 40 → "NEED TO IMPROVE"  
5. Print the corresponding grade message.  
6. End the program.



*Source Code:*
c
#include <stdio.h>
int main()
{
    int marks;
    scanf("%d", &marks);

    if (marks >= 70)
        printf("VERY GOOD");
    else if (marks >= 60)
        printf("GOOD");
    else if (marks >= 50)
        printf("ABOVE AVERAGE");
    else if (marks >= 40)
        printf("AVERAGE");
    else
        printf("NEED TO IMPROVE");

    return 0;
}

*output*

<img width="475" height="291" alt="image" src="https://github.com/user-attachments/assets/feb0daa9-8d10-43f7-a525-73cf950872b9" />

*Result:*

The program correctly evaluates the marks and displays the corresponding grade message.
