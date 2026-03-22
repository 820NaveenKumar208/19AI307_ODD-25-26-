# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class Circle that uses a constructor to calculate area using radius.

## AIM:
To write a Java program that defines a class Circle and uses a constructor to calculate the area using the given radius.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class named Circle.
4.	Declare variables radius and area.
5. Define a parameterized constructor.
6. Display the area inside the constructor.
7. In main(), create an object of Circle and pass the radius.






## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java

import java.util.Scanner;

class Circle {
   double area;

   // Constructor to calculate area
   Circle(double radius) {
       area = 3.14159 * radius * radius;
       System.out.printf("Area of the circle with radius %.2f is %.2f%n", radius, area);
   }
}

public class Main {
   public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);

       if (sc.hasNextDouble()) {           // check if input exists
           double radius = sc.nextDouble();
           Circle c = new Circle(radius);  // constructor calculates & prints area
       }

       // Do not close Scanner in online judges (prevents hidden test failures)
   }
}


```





## OUTPUT:
<img width="1113" height="173" alt="image" src="https://github.com/user-attachments/assets/219b3978-2634-4bfe-89f7-962e42c181b4" />



## RESULT:
The program successfully calculates and displays the area of a circle using a constructor.
