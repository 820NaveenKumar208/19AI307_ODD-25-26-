# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java Program to Find the Average of Array Elements.


## AIM:
To write a Java Program to Find the Average of Array Elements.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read an integer n from the user.
4.	Initialize factorial to 1.
5.	Use a loop from 1 to n, multiplying each value with factorial.
6.	Print the final factorial value and end the program.





## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java

import java.util.*;
public class Main {
    public static void main(String args[]) {
        Scanner input = new Scanner(System.in);
        
        int n = input.nextInt();
        int[] arr = new int[n];
        
        for(int i=0;i<n;i++) {
            arr[i] = input.nextInt();
        }
        
        int sum = 0;
        for(int i=0;i<n;i++) {
           sum += arr[i]; 
        }
        double avg = (double)sum/n;
        System.out.printf("The average of elements is %.2f",avg);
    }
} 

```





## OUTPUT:
<img width="1230" height="475" alt="image" src="https://github.com/user-attachments/assets/941621c1-7747-4e22-a386-cec4a6cde5a1" />



## RESULT:
The program successufully writes a Java Program to Find the Average of Array Elements.
