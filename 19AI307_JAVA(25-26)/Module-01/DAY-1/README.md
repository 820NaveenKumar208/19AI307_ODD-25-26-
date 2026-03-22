# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:

Lovely is preparing a countdown for her rocket launch game. She has a starting number and wants to understand how subtracting with -- works in Java. But she's puzzled by the two types:

Post-decrement (a--) → value is used first, then decreased

Pre-decrement (--a) → value is decreased first, then used

To complete the launch program, help Lovely:

Take a countdown number as input.

Apply both post-decrement and pre-decrement on it.

Show how the value changes in each case.


## AIM:  
To demonstrate the difference between pre-decrement (--a) and post-decrement (a--) in Java using a given countdown number.


## ALGORITHM :
1.	Start the program.
2. Read the countdown number as input.
3. Apply post-decrement (a--) and display the value before and after decrement.
4. Apply pre-decrement (--a) and display the updated value.
5. End the program.



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: 
RegisterNumber:  
*/
```

## Sourcecode.java:


```java

import java.util.*;
public class Main
{
    public static void main(String args[])
    {
        Scanner input = new Scanner(System.in);
        int n = input.nextInt();
        System.out.println("Initial countdown = "+n);
        System.out.println("After post-decrement (a--) = "+(n--)+", Now a = "+n);
        System.out.print("After pre-decrement (--a) = "+(--n)+", Now a = "+n);
    }
}

```




## OUTPUT:

<img width="1187" height="301" alt="image" src="https://github.com/user-attachments/assets/f468ec57-7db4-4065-bbb5-c050f8eab552" />


## RESULT:  Thus, the program successfully demonstrates the difference between post-decrement (a--) and pre-decrement (--a) by showing how the value changes in each case.
