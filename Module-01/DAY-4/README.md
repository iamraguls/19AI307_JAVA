# Ex.No:1(D) INSTANCE METHOD TO GET AND PRINT 2 VALUES

## AIM:
To write a Java method to get and print two values entered by the user by defining instance methods in the class 'Test'. The method names are `getData()` and `putData()`.

## ALGORITHM :
1. Start the program.
2. Define a class named 'Test' with two instance variables `num1` and `num2`.
3. Define the `getData()` method to read input values from the user.
4. Define the `putData()` method to print the values of `num1` and `num2`.
5. In the `main` method, create an object of the 'Test' class.
6. Call the `getData()` and `putData()` methods using the object.
7. End.

## PROGRAM:
```
/*
Program to get and print two values entered by the user using instance methods in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 1D_INSTANCE_METHOD_GET_PUT_DATA.JAVA:
```java
import java.util.*;

public class Test {
    
    int num1, num2;

    public void getData() {
        Scanner sc = new Scanner(System.in);
        num1 = sc.nextInt();
        num2 = sc.nextInt();
    }

    public void putData() {
        System.out.println("Number1 is: " + num1);
        System.out.println("Number2 is: " + num2);
    }

    public static void main(String[] args) {
        Test obj1 = new Test();

        obj1.getData();
        obj1.putData();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/21256776-5e34-47a1-951c-9113b07f95b4)


## RESULT:
Thus, the Java program to get and print two values entered by the user using instance methods was implemented and executed successfully.
