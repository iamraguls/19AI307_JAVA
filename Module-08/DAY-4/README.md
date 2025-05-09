# Ex.No:8(D) SUM OF NATURAL NUMBERS USING BUFFEREDREADER

## AIM:
To write a Java program to read the number from the user using the `BufferedReader` class and perform the sum of natural numbers.

## ALGORITHM:
1. Import necessary classes: `BufferedReader`, `InputStreamReader`, and `IOException`.
2. Read the input number using `BufferedReader`.
3. Use a loop to calculate the sum of natural numbers up to the given number.
4. Display the sum to the user.

## PROGRAM:
```
/*
Program to calculate the sum of first n natural numbers using BufferedReader.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 8D_SUM_OF_NATURAL_NUMBERS.JAVA:
```java
import java.io.*;

class Sample {
    void natural(int num) {
        int i, sum = 0;  
        for (i = 1; i <= num; ++i) {  
            sum = sum + i;  
        }  
        System.out.println("Sum of First " + num + " Natural Numbers is = " + sum);  
    }  
}

public class ReadData {
    public static void main(String args[]) throws IOException {
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
        int number = Integer.parseInt(reader.readLine());
        Sample std = new Sample();
        std.natural(number);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/194126e9-61db-40a7-adf9-3c46e29df241)

## RESULT:
The Java program to read the number from the user using `BufferedReader` class and calculate the sum of natural numbers was successfully executed.
