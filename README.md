# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <math.h>

void calculateEMI(float principal, float annualRate, int tenureMonths) {
    float monthlyRate = annualRate / (12 * 100); 
    float emi;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, tenureMonths)) /
          (pow(1 + monthlyRate, tenureMonths) - 1);

    printf("\nEMI for the loan is: ₹%.2f\n", emi);
}

int main() {
    float principal, rate;
    int tenure;
    printf("Enter the loan amount (principal): ₹");
    scanf("%f", &principal);

    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &rate);

    printf("Enter loan tenure (in months): ");
    scanf("%d", &tenure);

    calculateEMI(principal, rate, tenure);

    return 0;
}
```

## OUTPUT
![445607396-0fb0042c-05be-4740-8c0d-51559fde7107](https://github.com/user-attachments/assets/09535e86-5e88-4bb4-b3c4-29f4c675f98a)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n = 6; // Number of terms to generate
    int first = 0, second = 1, next;

    printf("Fibonacci Series for %d terms:\n", n);

    for (int i = 1; i <= n; i++) {
        printf("%d ", first);
        next = first + second;
        first = second;
        second = next;
    }

    return 0;
}

```
## OUTPUT
![445607680-fc3327ae-5fe2-460a-b892-adf8d2d5d0c4](https://github.com/user-attachments/assets/e7dbe3f6-ef50-4304-8325-64b2cde5dd86)








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int arr[100], n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element of the array is: %d\n", arr[n - 1]);
    return 0;
}
```
## OUTPUT

![445610515-03c97580-557d-4f41-90db-4ec1dfaf13a4](https://github.com/user-attachments/assets/5ee3cabd-7fb5-45a7-8446-83716a1430c5)








## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int arr[100], n, count = 0;

    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        if(arr[i] > 0) {
            count++;
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}

```

## OUTPUT

![445612736-04f81e27-139f-45b3-b9c4-15e69ccf195b](https://github.com/user-attachments/assets/b677b85b-e82b-4198-adf8-b4cda01bf616)




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```c
#include <stdio.h>

int main() {
    int arr[100], n;

    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    printf("Enter %d integer elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Modified array (even numbers replaced with 'E'):\n");
    for(int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");
    return 0;
}

```
## Output:
![445614165-1427e47a-ca1d-41c2-8fc6-f8c04730fda8](https://github.com/user-attachments/assets/02e97481-5a6b-471b-9d1f-5187b89339d8)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



