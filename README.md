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
```
#include <stdio.h>
#include <math.h>

// Function to calculate EMI (no return type, with arguments)
void calculateEMI(float principal, float annualRate, int tenureMonths) {
    float monthlyRate = annualRate / (12 * 100); // Convert annual rate to monthly and in decimal
    float emi;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, tenureMonths)) /
          (pow(1 + monthlyRate, tenureMonths) - 1);

    printf("\nEMI for the loan is: ₹%.2f\n", emi);
}

int main() {
    float principal, rate;
    int tenure;

    // Input values from user
    printf("Enter the loan amount (principal): ₹");
    scanf("%f", &principal);

    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &rate);

    printf("Enter loan tenure (in months): ");
    scanf("%d", &tenure);

    // Call the function
    calculateEMI(principal, rate, tenure);

    return 0;
}
```


## OUTPUT


![image](https://github.com/user-attachments/assets/0fb0042c-05be-4740-8c0d-51559fde7107)


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
```
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



![image](https://github.com/user-attachments/assets/fc3327ae-5fe2-460a-b892-adf8d2d5d0c4)




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
```
#include <stdio.h>

int main() {
    int arr[100], n;

    // Input: size of the array
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    // Input: elements of the array
    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Output: last element
    printf("The last element of the array is: %d\n", arr[n - 1]);

    return 0;
}


```


## OUTPUT
![image](https://github.com/user-attachments/assets/03c97580-557d-4f41-90db-4ec1dfaf13a4)









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
```
#include <stdio.h>

int main() {
    int arr[100], n, count = 0;

    // Input: number of elements
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    // Input: array elements
    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        // Count if the element is positive
        if(arr[i] > 0) {
            count++;
        }
    }

    // Output: total number of positive elements
    printf("Total number of positive elements: %d\n", count);

    return 0;
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/04f81e27-139f-45b3-b9c4-15e69ccf195b)





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
```
#include <stdio.h>

int main() {
    int arr[100], n;

    // Input: number of elements
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    // Input: array elements
    printf("Enter %d integer elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Output: Replace even elements with 'E'
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
 ![image](https://github.com/user-attachments/assets/1427e47a-ca1d-41c2-8fc6-f8c04730fda8)




## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



