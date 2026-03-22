# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a java program for determine the priority and name of the current thread.

## AIM:
To read a thread name from the user and display the current thread’s name and priority.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the thread name from the user.
4.	Get the reference of the current thread using Thread.currentThread().
5.	Set the name of the current thread using setName().
6.	Retrieve the thread’s name and priority using getName() and getPriority().
7.	Display both values.





## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java

import java.util.Scanner;

public class ThreadInfoExample {
   public static void main(String[] args) {
       Scanner scanner = new Scanner(System.in);

       // Read thread name from user
       String threadName = scanner.nextLine();

       // Create a thread with the given name
       Thread t = new Thread(() -> {
           // Thread work can go here if needed
       }, threadName);

       // Display priority and name
       System.out.println("Priority of Thread: " + t.getPriority());
       System.out.println("Name of Thread: " + t.getName());

       // Display full thread info (toString())
       System.out.println(t);

       scanner.close();
   }
}

```





## OUTPUT:
<img width="1115" height="148" alt="image" src="https://github.com/user-attachments/assets/0e8dc7c0-ef84-4fe5-8ec1-89b5d0c251b1" />



## RESULT:
The program successfully reads the thread name from the user and displays the current thread’s name and priority.
