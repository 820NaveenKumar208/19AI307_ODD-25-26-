# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a Java program to write characters to a file using FileWriter.

## AIM:
To write character data into a file using the FileWriter class in Java.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Import java.io.FileWriter and java.io.IOException.
4.	Create a FileWriter object with the desired file name.
5.	Use write() method to write text into the file.
6.	Close the FileWriter and handle exceptions using try-catch.






## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java


import java.io.*;

public class FileWriteExample {
   public static void main(String[] args) {
       try {
           BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
           String filename = br.readLine();
           String content = br.readLine();

           FileWriter fw = new FileWriter(filename);
           fw.write(content);
           fw.close();

           System.out.println("File written successfully.");
       } catch (IOException e) {
           System.out.println("An error occurred.");
       }
   }
}

```





## OUTPUT:
<img width="1108" height="255" alt="image" src="https://github.com/user-attachments/assets/1fcb7f9c-26dd-4f52-bc7b-3a8bcc030e54" />



## RESULT:
The program successfully writes the entered text into output.txt using FileWriter.
