# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to calculate the factorial of a number using a for loop. The factorial of n is the product of all positive integers less than or equal to n.


## AIM:
To write a Java program to calculate the factorial of a number using a for loop.


## ALGORITHM :
1. Start the program.
2. Import the necessary package 'java.util'.
3. Read an integer n from the user.
4. Initialize factorial to 1.
5. Use a loop from 1 to n, multiplying each value with factorial.
6. Print the final factorial value and end the program.





## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java
import java.util.*;
public class Main
{
    public static void main(String args[])
    {
        Scanner input = new Scanner(System.in);
        int n = input.nextInt();
        if(n == 0)
        {
            System.out.print("Factorial of "+n+" is: 1");
        }
        else
        {
            int f = 1;
            for(int i=n;i>0;i--)
            {
                f*=i;
            }
            System.out.print("Factorial of "+n+" is: "+f);
        }
    }
}

```





## OUTPUT:
<img width="1239" height="255" alt="image" src="https://github.com/user-attachments/assets/0467b8d7-bbe4-45be-8c43-c5738ea7f166" />



## RESULT:
The program successfully writes a Java program to calculate the factorial of a number using a for loop.
