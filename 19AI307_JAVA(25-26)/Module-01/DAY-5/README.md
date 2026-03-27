# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To write a Java program to reverse a given string.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read a string input from the user.
4.	Initialize an empty string reversed.
5.	Traverse the original string from end to start and append each character to reversed.
6.	Print the reversed string and end the program.

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Naveen Kumar T
RegisterNumber: 212223220067
*/
```

## SOURCE CODE:
```java

import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        
        String str = input.nextLine();
        int len = str.length();
        
        System.out.print("Reversed string: ");
        
        for(int i = len-1; i >= 0; i--) {
            System.out.print(str.charAt(i));
        }
    }
}

```


## OUTPUT:
<img width="1234" height="250" alt="image" src="https://github.com/user-attachments/assets/3e05f97d-ea01-43f7-9064-dfc4867c47f7" />



## RESULT:
The program successfully writes a Java program to reverse a given string.
