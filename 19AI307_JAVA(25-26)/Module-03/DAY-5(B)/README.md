# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to convert a string to an integer using a wrapper class and perform addition.

## AIM:
To convert string inputs into integers using the wrapper class and perform addition.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read two numbers as strings.
4.	Convert them to integers using Integer.parseInt().
5.	Add the two integers.
6.	Display the sum.





## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java
import java.util.Scanner;

public class Main {
   public static void main(String[] args) {
       Scanner scanner = new Scanner(System.in);

       String str1 = scanner.next();

       String str2 = scanner.next();

       scanner.close();

       try {
           int num1 = Integer.parseInt(str1);
           int num2 = Integer.parseInt(str2);


           int sum = num1 + num2;
           System.out.println("Sum = " + sum);
       } catch (NumberFormatException e) {
           System.out.println("Invalid input. Please enter a valid number.");
       }
   }
}


```





## OUTPUT:
<img width="1109" height="275" alt="image" src="https://github.com/user-attachments/assets/d7bc0003-ff17-4423-9d60-430d738bc29b" />



## RESULT:
The program successfully converts strings to integers and displays their sum.
