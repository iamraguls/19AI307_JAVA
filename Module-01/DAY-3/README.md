# Ex.No:1(C) SUM AND AVERAGE USING WHILE LOOP

## AIM:
To write a Java program to input 5 numbers from the keyboard and calculate their sum and average using a while loop.

## ALGORITHM :
1. Start the program.
2. Import the `Scanner` class to read input from the user.
3. Initialize a variable `n` to 0 for the sum and `i` for reading the input.
4. Use a `while` loop to take 5 numbers as input.
5. Calculate the sum of the entered numbers.
6. Calculate the average by dividing the sum by 5.
7. Display the sum and average.
8. End.

## PROGRAM:
```
/*
Program to calculate the sum and average of 5 numbers using a while loop in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 1C_SUM_AND_AVERAGE_WHILE_LOOP.JAVA:
```java
import java.util.*;
public class Main {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int i, n = 0;
        int count = 0;
        
        while(count < 5) {
            i = sc.nextInt();
            n = n + i;
            count++;
        }

        System.out.println("The sum of 5 no is : " + n);
        float a = n / 5.0f;
        System.out.printf("The Average is : %.1f", a);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/9dc8df67-17a2-4138-85a4-a9c70247e305)


## RESULT:
Thus, the Java program to input 5 numbers and calculate their sum and average using a while loop was implemented and executed successfully.
