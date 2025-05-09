# Ex.No:5(C) FACTORIAL USING SETTER AND GETTER

## AIM:
To write a Java program that prints the factorial of a given number using setter and getter methods.

## ALGORITHM :
1. Start the program.
2. Create a class `FactorialCalculator` with private variables `number` and `factorial`.
3. Implement setter method `setNumber()` to set the number and calculate factorial.
4. Implement getter methods `getNumber()` and `getFactorial()` to access number and factorial.
5. In the `Main` class, read a number from the user.
6. Use `setNumber()` to set the input and calculate factorial.
7. Print the result using getter methods.
8. End.

## PROGRAM:
```
/*
Program to calculate factorial using setter and getter methods in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 5C_FACTORIAL_SET_GET.JAVA:
```java
import java.util.Scanner;

class FactorialCalculator {
    private int number;
    private long factorial;

    public void setNumber(int number) {
        this.number = number;
        calculateFactorial();
    }

    public int getNumber() {
        return number;
    }

    public long getFactorial() {
        return factorial;
    }

    private void calculateFactorial() {
        factorial = 1;
        for (int i = 1; i <= number; i++) {
            factorial *= i;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        FactorialCalculator fc = new FactorialCalculator();

        int num = scanner.nextInt();
        fc.setNumber(num);

        System.out.println("Factorial of " + fc.getNumber() + " is: " + fc.getFactorial());

        scanner.close();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/27ae009e-23e9-4e8c-8298-004265006362)


## RESULT:
Thus, the Java program to find the factorial of a number using setter and getter methods was successfully implemented and executed.
