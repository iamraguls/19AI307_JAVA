# Ex.No:5(B) TIGHTLY ENCAPSULATED CLASS TO CALCULATE SUM OF TWO NUMBERS

## AIM:
To demonstrate the use of a tightly encapsulated class in Java that reads string inputs and calculates the sum of two numbers.

## ALGORITHM:
1. Define a nested static class `Multi` with private integer fields `n1` and `n2`.
2. Use a method `setValues()` to convert and set input values from string to integers.
3. Use a method `getProd()` to return the sum of the two numbers.
4. Read inputs as strings in the main method and use the class to calculate and print the sum.

## PROGRAM:

### 5B_TIGHT_ENCAPSULATION_SUM.JAVA:
```
/*
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```
```java
import java.util.*;

public class Pro {
    public static class Multi {
        private int n1;
        private int n2;

        public void setValues(String num1, String num2) {
            this.n1 = Integer.parseInt(num1);
            this.n2 = Integer.parseInt(num2);
        }

        public int getProd() {
            return n1 + n2;
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String str1 = sc.nextLine();
        String str2 = sc.nextLine();

        Multi multi = new Multi();
        multi.setValues(str1, str2);
        int pro = multi.getProd();
        System.out.println("Sum is " + pro);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c323dd2a-b2a2-4caf-9c17-f550ffc840e7)


## RESULT:
The Java program successfully uses a tightly encapsulated class to read input in string format and print the sum of two numbers.
