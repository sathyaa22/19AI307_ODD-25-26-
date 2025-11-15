# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to calculate the power of a given number.

## AIM:
To write a Java program to calculate the power of a given number.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the base value from the user.
4.	Read the exponent value from the user.
5.	Initialize a variable result to store the final answer.
6.	Compute the power using the formula: result = Math.pow(base, exponent).
7.	Store the computed value in result.
8.	Display the message: base raised to exponent is result.
9.	End the program.


## PROGRAM:

```
Program to implement a Strings and Math Function using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

public class PowerCalculator 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);

        double base = sc.nextDouble();
        double exponent = sc.nextDouble();
        double result = Math.pow(base, exponent);
        
        System.out.println(base + " raised to the power of " + exponent + " is: " + result);
        sc.close();
    }
}
```

## OUTPUT:

<img width="999" height="268" alt="image" src="https://github.com/user-attachments/assets/ecdf8426-ed9a-482f-82f6-1eb38d8c8785" />


## RESULT:
Thus, the program to write a Java program to calculate the power of a given number is written and executed successfully.
