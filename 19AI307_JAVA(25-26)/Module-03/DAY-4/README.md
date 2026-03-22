# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.

Bot Types:

SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".

RainBot: Predicts "COLD" if temperature < 20, else "WARM".

Input:

temperature botType (1 for SunBot, 2 for RainBot)Output: Prediction as a string.

## AIM:
To implement weather prediction using interfaces with two bots — SunBot and RainBot.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3. Create WeatherBot interface with predict() method.
4. Implement SunBot and RainBot classes with different prediction logic.
5. Take temperature and botType as input.
6. Use the chosen bot to call predict().
7. Display the prediction.	





## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```java
import java.util.Scanner;

interface WeatherBot {
   String predict(int temperature);
}

class SunBot implements WeatherBot {
   public String predict(int temperature) {
       if (temperature > 30) {
           return "HOT";
       } else {
           return "MODERATE";
       }
   }
}

class RainBot implements WeatherBot {
   public String predict(int temperature) {
       if (temperature < 20) {
           return "COLD";
       } else {
           return "WARM";
       }
   }
}

public class Main {
   public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int temperature = sc.nextInt();
       int botType = sc.nextInt();
       WeatherBot bot;

       if (botType == 1) {
           bot = new SunBot();
       } else {
           bot = new RainBot();
       }

       System.out.println(bot.predict(temperature));
       sc.close();
   }
}

```





## OUTPUT:
<img width="1092" height="189" alt="image" src="https://github.com/user-attachments/assets/e82db369-ddba-4cb8-8252-b3e3f42b698c" />



## RESULT:
The program predicts weather conditions using interface implementation and method overriding.
