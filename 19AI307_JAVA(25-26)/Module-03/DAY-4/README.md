# Ex.No:3(D)    INTERFACE 

## QUESTION:
Each judge uses different criteria to score fighters. Based on points, the judge will declare “WIN”, “LOSE” or “DRAW”.

LenientJudge: WIN if diff ≥ 5, DRAW if < 5

StrictJudge: WIN if diff ≥ 10, DRAW if < 10

Input Format:

player1Score
player2Score
judgeType
player1Score, player2Score: integers

judgeType: 1 for LenientJudge, 2 for StrictJudge

Output Format:
WIN / LOSE / DRAW


## AIM:
To write a java program that evaluates two fighters’ scores using selected judging criteria to decide whether the result is WIN, LOSE, or DRAW.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define an interface BoxingJudge with the method decide(p1, p2).
4.	Implement two classes: LenientJudge (win if diff ≥ 5) and StrictJudge (win if diff ≥ 10), each providing its own version of decide().
5.	In the main() method, read player1Score, player2Score, and judgeType from the user.
6.	Based on judgeType, create either a LenientJudge or StrictJudge object.
7.	Call the decide() method with the two scores to determine WIN / LOSE / DRAW.
8.	Print the result
9.	End the program.


## PROGRAM:

```
Program to implement a Interface using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.*;

interface BoxingJudge 
{
    String decide(int p1, int p2);
}

class LenientJudge implements BoxingJudge 
{
    public String decide(int p1, int p2) 
    {
        if (Math.abs(p1 - p2) >= 5)
            return (p1 > p2) ? "WIN" : "LOSE";
        return "DRAW";
    }
}

class StrictJudge implements BoxingJudge 
{
    public String decide(int p1, int p2) 
    {
        if (Math.abs(p1 - p2) >= 10)
            return (p1 > p2) ? "WIN" : "LOSE";
        return "DRAW";
    }
}

public class prog 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt();
        int type = sc.nextInt();
        BoxingJudge judge = (type == 1) ? new LenientJudge() : new StrictJudge();
        System.out.println(judge.decide(a, b));
    }
}
```


## OUTPUT:

<img width="369" height="325" alt="image" src="https://github.com/user-attachments/assets/784816eb-4379-40d4-a5f9-d26054d9fc55" />


## RESULT:
Thus, the program that evaluates two fighters’ scores using selected judging criteria to decide whether the result is WIN, LOSE, or DRAW is written and execited successfully.
