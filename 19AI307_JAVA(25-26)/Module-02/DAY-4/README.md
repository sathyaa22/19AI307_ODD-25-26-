# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a program to demonstrate the use of a default constructor and display a message from it.

## AIM:
To write a program to demonstrate the use of a default constructor and display a message from it.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util' and create a Scanner to read user input.
3.	Call the constructor of the WelcomeDemo class while passing the user-entered name.
4.	Inside the constructor, assign the passed name to the instance variable.
5.	Print a welcome message from the constructor.
6.	Return control to main()
7.	End the program.


## PROGRAM:

```
Program to implement a Variable scope and Constructor using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

public class WelcomeDemo 
{
    String name;
    WelcomeDemo(String name) 
    {
        this.name = name;
        System.out.println("Welcome, " + name + "! This is the default constructor.");
    }

    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        String inputName = sc.nextLine();
        sc.close();
        
        new WelcomeDemo(inputName);
    }
}
```


## OUTPUT:

<img width="1583" height="365" alt="image" src="https://github.com/user-attachments/assets/a943b261-a22c-49a5-8d59-bd4c64410a28" />


## RESULT:
Thus, the program to demonstrate the use of a default constructor and display a message from it is written and executed successfully.
