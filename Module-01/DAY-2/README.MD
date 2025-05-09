# Ex.No:1(B) TOTAL AND PERCENTAGE CALCULATION

## AIM:
To write a Java program to calculate total and percentage marks obtained by Robert in three subjects.

## ALGORITHM :
1. Start the program.
2. Import the `Scanner` class to read input from the user.
3. Read three float values representing the marks in three subjects.
4. Calculate the total by summing the three values.
5. Calculate the percentage by dividing the total by 3.
6. Display the total and percentage.
7. End.

## PROGRAM:
```
/*
Program to calculate total and percentage marks using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 1B_TOTAL_AND_PERCENTAGE.JAVA:
```java
import java.util.*;
public class main {
    public static void main(String[] args){
        
        Scanner sc = new Scanner(System.in);
        float a = sc.nextInt();
        float b = sc.nextInt();
        float c = sc.nextInt();
        
        float total = a + b + c;
        
        double percentage = (total / 3.0);

        System.out.println("Total marks (out of 300): " + total);
        System.out.println("Percentage: " + percentage + "%");
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/41909aad-0af3-4497-80fd-9fe5a5ca3721)


## RESULT:
Thus, the Java program to calculate total and percentage marks for three subjects was implemented and executed successfully.
