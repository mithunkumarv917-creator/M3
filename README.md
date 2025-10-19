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
void calculateEMI(float principal, float rate, int months) {
    float r, emi;
    r = rate / (12 * 100);

    emi = (principal * r * pow(1 + r, months)) / (pow(1 + r, months) - 1);
    printf("Monthly EMI = %.2f\n", emi);
}
int main() {
    float principal, rate;
    int months;
    scanf("%f", &principal);
    scanf("%f", &rate);
    scanf("%d", &months);
    calculateEMI(principal, rate, months);
    return 0;
}

```


## OUTPUT


<img width="1918" height="873" alt="image" src="https://github.com/user-attachments/assets/a89d3c49-c0a1-4bd7-b341-81bde60d040e" />




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
    int n;                  
    int t1 = 0, t2 = 1;   
    int nextTerm;           

    scanf("%d", &n);
    printf("Fibonacci Series: %d %d ", t1, t2);

    for (int i = 3; i <= n; i++) {
        nextTerm = t1 + t2;
        printf("%d ", nextTerm);
        t1 = t2;
        t2 = nextTerm;
    }

    return 0;
}

```

## OUTPUT

<img width="1918" height="872" alt="image" src="https://github.com/user-attachments/assets/967d0c77-4e7f-4708-a80e-be86d800ca22" />








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
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    int arr[n];

    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    
    printf("The Last number is %d",arr[n-1]);
    
}
```

## OUTPUT





<img width="1918" height="871" alt="image" src="https://github.com/user-attachments/assets/6a929ce5-d561-4094-a027-de6ebc9c4b88" />





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
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    int arr[n];
    int count =0;
    
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<n;i++){
        if(arr[i]%2==0){
            count++;
        }

    }
    printf("The total number of Positive are %d",count);
    
}
```


## OUTPUT

<img width="1918" height="882" alt="image" src="https://github.com/user-attachments/assets/875c01b1-28ee-4bd9-93bc-5c1f6956875f" />






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
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    int arr[n];
    
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<n;i++){
        if(arr[i]%2==0){
          printf("E ");
        }
        else{
            printf("%d ",arr[i]);
        }
    }
    
}
```

## Output:
 
<img width="1918" height="876" alt="image" src="https://github.com/user-attachments/assets/03e2650d-1bb8-4efb-b81f-9c97e94886a0" />


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



