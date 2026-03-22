# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:
Write a Java program to read a string from the user, compress it in memory using ByteArrayOutputStream + GZIPOutputStream, and then decompress it back using ByteArrayInputStream + GZIPInputStream.

## AIM:
To demonstrate string compression and decompression using ByteArrayOutputStream, GZIPOutputStream, ByteArrayInputStream, and GZIPInputStream.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read a string from the user.
4.	Create a ByteArrayOutputStream and wrap it in a GZIPOutputStream to compress the string.
5.	Convert the compressed output to a byte array.Use ByteArrayInputStream and GZIPInputStream to decompress the byte array back to the original string.
6.	Display both compressed size and decompressed string.





## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java

import java.io.*;
import java.util.Scanner;
import java.util.zip.GZIPOutputStream;
import java.util.zip.GZIPInputStream;

public class GZIPMemoryExample {
   public static void main(String[] args) {
       Scanner scanner = new Scanner(System.in);

       try {
           // Get input string from user
           String input = scanner.nextLine();

           // --- Compress the string ---
           ByteArrayOutputStream baos = new ByteArrayOutputStream();
           GZIPOutputStream gzipOut = new GZIPOutputStream(baos);
           gzipOut.write(input.getBytes("UTF-8"));
           gzipOut.close(); // Finish compression

           byte[] compressedData = baos.toByteArray();
           System.out.println("Compressed data (bytes):");
           for (byte b : compressedData) {
               System.out.print(b + " ");
           }
           System.out.println("\nTotal bytes: " + compressedData.length);

           // --- Decompress the string ---
           ByteArrayInputStream bais = new ByteArrayInputStream(compressedData);
           GZIPInputStream gzipIn = new GZIPInputStream(bais);
           InputStreamReader reader = new InputStreamReader(gzipIn, "UTF-8");
           BufferedReader br = new BufferedReader(reader);

           StringBuilder decompressed = new StringBuilder();
           String line;
           while ((line = br.readLine()) != null) {
               decompressed.append(line);
           }

           System.out.println("\nDecompressed string:");
           System.out.println(decompressed.toString());

       } catch (IOException e) {
           System.out.println("Error: " + e.getMessage());
       }

       scanner.close();
   }
}

```





## OUTPUT:
<img width="1117" height="434" alt="image" src="https://github.com/user-attachments/assets/15fd93e8-b8dc-4ab5-82cb-cca3245459c3" />



## RESULT:
The program successfully compresses and decompresses a string in memory using GZIP streams, showing reduced data size and restoring the original text accurately.
