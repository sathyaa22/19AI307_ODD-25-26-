# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Rectangle with private instance variables length and width. Provide public getter and setter methods to access and modify these variables.

## AIM:
To write a Java program that defines a Rectangle class with private fields and public getters and setters.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util' and create a Scanner object to read input.
3.	Create a Rectangle object.
4.	Read the length from the user and store it using setLength().
5.	Read the width from the user and store it using setWidth().
6.	Retrieve the stored length and width using the getter methods.
7.	Display the length and width.
8.	End the program.



## PROGRAM:

```
Program to implement a Access Specifiers using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

class Rectangle 
{
    private double length;
    private double width;

    public double getLength() 
    {
        return length;
    }
    public void setLength(double length) 
    {
        this.length = length;
    }
    public double getWidth() 
    {
        return width;
    }
    public void setWidth(double width) 
    {
        this.width = width;
    }
    public double calculateArea() 
    {
        return length * width;
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner scanner = new Scanner(System.in);
        Rectangle rect = new Rectangle();

        double length = scanner.nextDouble();
        rect.setLength(length);
        double width = scanner.nextDouble();
        rect.setWidth(width);

        System.out.println("Length: " + rect.getLength());
        System.out.println("Width: " + rect.getWidth());

        scanner.close();
    }
}
```


## OUTPUT:

<img width="570" height="409" alt="image" src="https://github.com/user-attachments/assets/38b436c3-1b5d-4c94-b705-93b5edb93f76" />


## RESULT:
Thus, the program that defines a Rectangle class with private fields and public getters and setters is written and executed successfully.
