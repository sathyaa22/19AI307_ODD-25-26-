# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to find the sum of even and odd elements in an array.

## AIM:
To write a Java program to find the sum of even and odd elements in an array.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the size of the array n from the user.
4.	Create an array of size n and read all n elements into it.
5.	Initialize two variables: sumEven = 0 and sumOdd = 0.
6.	Repeat for each element in the array:
   a. If the element is even, add it to sumEven.
  	b. Else, add it to sumOdd.
7. Display sumEven and sumOdd
8. End the program.


## PROGRAM:

```
Program to implement a Array concept using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

public class SumEvenOdd 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++) 
        {
            arr[i] = sc.nextInt();
        }
        
        int sumEven = 0;
        int sumOdd = 0;

        for (int num : arr) 
        {
            if (num % 2 == 0) 
            {
                sumEven += num;
            } 
            else 
            {
                sumOdd += num;
            }
        }
        System.out.println("Sum of even elements: " + sumEven);
        System.out.println("Sum of odd elements: " + sumOdd);
        sc.close();
    }
}
```

## OUTPUT:

<img width="700" height="663" alt="image" src="https://github.com/user-attachments/assets/1514a5ff-bfc3-431a-9899-c6bf88776242" />


## RESULT:
Thus, the program to write a Java program to find the sum of even and odd elements in an array is written and executed successfully.
