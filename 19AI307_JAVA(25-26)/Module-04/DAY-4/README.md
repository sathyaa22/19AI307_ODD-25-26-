# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
Create a program that loads an operating system shell using the Factory Pattern. Based on user input, return a shell object: windows, linux, mac.

## AIM:
To write a java program that implements a Factory returning a Windows, Linux, or Mac shell object based on user input.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the operating system name from the user inside a loop.
4.	Pass the input to the ShellFactory to request the appropriate shell object.
5.	Inside the factory, check the OS name and return the matching shell implementation.
6.	If a valid shell is returned, call its loadShell() method.
7.	If no matching object exists, print an error message for invalid OS input.
8.	Repeat until the user types "exit".
9.	End the program.


## PROGRAM:

```
Program to implement a Abstract Factory Pattern using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

interface Shell {
    void loadShell();
}

class WindowsShell implements Shell {
    public void loadShell() {
        System.out.println("Loading Windows Shell");
    }
}

class LinuxShell implements Shell {
    public void loadShell() {
        System.out.println("Loading Linux Shell");
    }
}

class MacShell implements Shell {
    public void loadShell() {
        System.out.println("Loading Mac Shell");
    }
}

class ShellFactory {
    public Shell getShell(String os) {
        if (os.equalsIgnoreCase("linux")) {
            return new LinuxShell();
        } else if (os.equalsIgnoreCase("mac")) {
            return new MacShell();
        }
        return null;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        ShellFactory factory = new ShellFactory();
        while (true) {
            String input = sc.nextLine();
            if (input.equalsIgnoreCase("exit")) break;
            Shell shell = factory.getShell(input);
            if (shell != null) shell.loadShell();
            else System.out.println("Invalid OS: " + input);
        }
    }
}
```


## OUTPUT:

<img width="619" height="342" alt="image" src="https://github.com/user-attachments/assets/4f787401-c9d0-4a8b-8c01-8008ba1233bd" />


## RESULT:
Thus, the program that implements a Factory returning a Windows, Linux, or Mac shell object based on user input is written and executed successfully.
