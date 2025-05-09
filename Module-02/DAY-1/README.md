# Ex.No:2(A) CUBE OF A NUMBER USING STATIC METHOD

## AIM:
To write a Java program to calculate the cube of a number using a static method.

## ALGORITHM :
1. Start the program.
2. Import the `Scanner` class to read input from the user.
3. Define a static method `cube()` that takes an integer as input and calculates its cube.
4. In the `main` method, create a `Scanner` object to take the input number.
5. Call the `cube()` method to compute the cube of the entered number.
6. Display the result.
7. End.

## PROGRAM:
```
/*
Program to calculate the cube of a number using a static method in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 2A_CUBE_OF_A_NUMBER_STATIC_METHOD.JAVA:
```java
import java.util.*;

public class main {
    public static void cube(int n){
        int cube = (int) Math.pow(n, 3);
        System.out.print("Cube is: " + cube);
    }

    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        cube(n);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/fafbef88-d4ff-4be3-b3a8-7f50f7f07a34)




## RESULT:
Thus, the Java program to calculate the cube of a number using a static method was implemented and executed successfully.
