# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create an abstract class TaxPayer with method calculateTax(). Create subclasses SalariedPerson and BusinessPerson.

## AIM:
To write a java program to create an abstract class TaxPayer with method calculateTax() and to create subclasses SalariedPerson and BusinessPerson.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define an abstract class TaxPayer with an abstract method calculateTax() and a constructor to store income.
4.	Create two subclasses SalariedPerson and BusinessPerson, each implementing calculateTax() with different tax rates (10% and 15%).
5.	In the main() method, read the taxpayer type (1 for salaried, 2 for business) and income from the user.
6.	Based on the type, create either a SalariedPerson or BusinessPerson object.
7.	Call the calculateTax() method on the created object to compute tax.
8.	Print the calculated tax amount.
9.	End the program.


## PROGRAM:

```
Program to implement a Abstraction using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.*;

abstract class TaxPayer 
{
    double income;
    TaxPayer(double income) 
    {
        this.income = income;
    }
    abstract double calculateTax();
}
class SalariedPerson extends TaxPayer 
{
    SalariedPerson(double income) 
    {
        super(income);
    }
    @Override
    double calculateTax() 
    {
        return income * 0.10;
    }
}
class BusinessPerson extends TaxPayer 
{
    BusinessPerson(double income) 
    {
        super(income);
    }
    @Override
    double calculateTax() 
    {
        return income * 0.15;
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int type = sc.nextInt();
        double income = sc.nextDouble();

        TaxPayer person;
        if (type == 1) 
        {
            person = new SalariedPerson(income);
        } 
        else 
        {
            person = new BusinessPerson(income);
        }
        System.out.printf("%.2f\n", person.calculateTax());
    }
}
```


## OUTPUT:

<img width="397" height="412" alt="image" src="https://github.com/user-attachments/assets/1790b157-ebde-497b-8b92-9dfa1d0afe68" />


## RESULT:
Thus, the program to create an abstract class TaxPayer with method calculateTax() and to create subclasses SalariedPerson and BusinessPerson is written and executed successfully.
