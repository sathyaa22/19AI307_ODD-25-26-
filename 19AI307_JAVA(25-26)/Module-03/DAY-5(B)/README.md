# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class. Take input from the user.

## AIM:
To write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read a number from the user and count its digits using Integer.toString(num).length().
4.	Copy the number into a temporary variable and set sum = 0.
5.	Extract each digit using temp % 10.
6.	Add Math.pow(digit, digits) to sum.
7.	Divide temp by 10 and repeat steps 3–4 until all digits are processed.
8.	Compare sum with the original number and print whether it is an Armstrong number.
9.	End the program.


## PROGRAM:

```
Program to implement a Wrapper Class using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

public class ArmstrongNumber
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        int digits = Integer.toString(num).length();
        
        int temp = num;
        int sum = 0;
        
        while (temp > 0) 
        {
            int digit = temp % 10;
            sum += Math.pow(digit, digits);
            temp /= 10;
        }
        if (sum == num) 
        {
            System.out.println(num + " is an Armstrong number.");
        } 
        else 
        {
            System.out.println(num + " is not an Armstrong number.");
        }
        sc.close();
    }
}
```


## OUTPUT:

<img width="839" height="270" alt="image" src="https://github.com/user-attachments/assets/54f76d5a-ccff-46bd-8f1c-bc26dc01a1ab" />


## RESULT:
Thus, the program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class is written and executed successfully.
