# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A library charges a fine for every book returned late. For first 5 days the fine is 50 paise, for 6-10 days fine is one rupee and above 10 days fine is 5 rupees. If you return the book after 30 days your membership will be cancelled - Print ("Your Membership would be Cancelled.")

Write a program to accept the number of days the member is late to return the book and display the fine or the appropriate message.

## AIM:
To write a java program to accept the number of days the member is late to return the book and display the fine or the appropriate message.

## ALGORITHM :
1.	Start the program.
2.	Read the number of late days from the user.
3.	If days ≤ 5, set fine = days × 0.50
4.	Else if days ≤ 10, set fine = days × 1
5.	Else if days ≤ 30, set fine = days × 5
6.	If days > 30, display “Your Membership would be Cancelled” and stop.
7.	Display the calculated fine.
8.	End the program.


## PROGRAM:

```
Program to implement a conditional statement using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

public class LibraryFine
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int days = sc.nextInt();
        sc.close();
        double fine;

        if (days <= 5)
        {
            fine = days * 0.50;
        }
        else if (days <= 10)
        {
            fine = days * 1.0; 
        }
        else
        {
            fine = days * 5.0; 
        }
        System.out.printf("Fine Amount Pay to Rs :%.2f\n", fine);
        if (days > 30)
        {
            System.out.println("Your Membership would be Cancelled.");
        }
    }
}
```

## OUTPUT:

<img width="920" height="246" alt="Screenshot 2025-11-15 111815" src="https://github.com/user-attachments/assets/80e243cf-b4ed-4e4a-87f3-8cfdd880c3aa" />


## RESULT:
Thus, the program to accept the number of days the member is late to return the book and display the fine is written and executed successfully.
