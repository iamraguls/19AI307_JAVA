# Ex.No:5(D) FACTORIAL USING CLASS, OBJECT, AND HAS-A RELATIONSHIP

## AIM:
To write a Java program to find the factorial of a number using class and object concepts and apply the has-a relationship.

## ALGORITHM :
1. Start the program.
2. Define a class `FactorialCalculator` with a method `fact(int num)` that calculates factorial recursively.
3. In the `Main` class, create an instance of `FactorialCalculator` (has-a relationship).
4. Read input from the user.
5. Call the `fact()` method using the object and store the result.
6. Display the factorial.
7. End.

## PROGRAM:
```
/*
Program to find factorial using class, object, and has-a relationship in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 5D_FACTORIAL_HAS_A.JAVA:
```java
import java.util.Scanner;

class FactorialCalculator {
    public int fact(int num) {
        if(num==1){
            return 1;
        }
        return fact(num-1)*num;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        FactorialCalculator calculator = new FactorialCalculator(); 

        int number = scanner.nextInt();
        int result = calculator.fact(number);

        System.out.println("Factorial is:" + result);

        scanner.close();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/38ad7766-20a7-4e2d-b4a3-b8ebebf95485)


## RESULT:
Thus, the Java program to find the factorial using class, object, and has-a relationship was successfully implemented and executed.
