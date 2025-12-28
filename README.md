# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:

#include <stdio.h>
int main() 
{

    printf("Integer Literal: %d\n", 42);
    printf("Float Literal: %f\n", 3.14159);
    printf("Float Literal (two decimals): %.2f\n", 3.14159);
    printf("Character Literal: %c\n", 'A');
    printf("String Literal: %s\n", "Hello, C Programming!");
    return 0;
}

# Output:
<img width="1243" height="352" alt="image" src="https://github.com/user-attachments/assets/932cf1f0-6dfc-44c1-b66b-71a5d69d8b03" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable. 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
#include<stdio.h>

#define PI 3.14159

int main()
{

    const int DAYS = 7;
    printf("Value of PI is %f\n",PI);
    printf("Value of DAYS is %d\n",DAYS);
    return 0;
}

# Output:
<img width="1202" height="353" alt="image" src="https://github.com/user-attachments/assets/9eb6f495-8b7a-4c8e-93ac-b04e80a00855" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
#include <stdio.h>
int main() 
{

    int integer_value = 10;
    float float_value = 3.14;  
    double double_value = 3.14;
    char char_value = 'A';
    printf("Integer Value: %d\n", integer_value);
    printf("Float Value: %f\n", float_value);  
    printf("Double Value: %lf\n", double_value); 
    printf("Character Value: %c\n", char_value);
    return 0;
}

# Output:
<img width="1203" height="457" alt="image" src="https://github.com/user-attachments/assets/f7c0536e-92d2-4f49-8bab-8fe6efaf5faf" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
#include <stdio.h>
int main() {

    int num1, num2;
    scanf("%d%d",&num1,&num2);
    printf("\n*** Arithmetic Operations ***\n");
    printf("Addition (%d + %d) = %d\n",num1,num2,num1+num2);
    printf("Subtraction (%d - %d) = %d\n",num1,num2,num1-num2);
    printf("Multiplication (%d * %d) = %d\n",num1,num2,num1*num2);
    printf("Division (%d / %d) = %d\n",num1,num2,num1/num2);
    printf("Remainder (%d %% %d) = %d\n",num1,num2,num1%num2);
    printf("\n*** Bitwise Operations ***\n");
    printf("Bitwise AND (%d & %d) = %d\n", num1, num2, num1 & num2);
    printf("Bitwise OR (%d | %d) = %d\n", num1, num2, num1 | num2);
    printf("Bitwise XOR (%d ^ %d) = %d\n", num1, num2, num1 ^ num2);
    printf("Bitwise Left Shift (%d << 1) = %d\n", num1, num1 << 1);
    printf("Bitwise Right Shift (%d >> 1) = %d\n", num1, num1 >> 1);
    printf("Bitwise NOT (~%d) = %d\n", num1, ~num1);
    printf("Bitwise NOT (~%d) = %d\n", num2, ~num2);
    return 0;
}
# Output:
<img width="1196" height="632" alt="image" src="https://github.com/user-attachments/assets/d7c59e0d-819e-452b-8d8d-3dfdb4e16c75" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
#include<stdio.h>
int main()
{

    char ch;
    scanf("%c",&ch);
    if(ch >= '0'&& ch <='9'){
        printf("Digit.");
    }else{
        if( (ch >= 'A'&& ch <= 'Z') || (ch >= 'a'&& ch <= 'z') ){
            if(ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'){
                printf("Vowel.");
            }else{
                printf("Consonant.");
            }
        }else{
            printf("Special Character.");
        }
    }
    return 0;
}
# Output:
<img width="1375" height="638" alt="image" src="https://github.com/user-attachments/assets/86d5cf57-586c-4f17-873f-7f72ede60762" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


