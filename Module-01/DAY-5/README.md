# Ex.No:1(E) SWAPPING VALUES WITHOUT A THIRD VARIABLE

## AIM:
To write a Java program to swap the values of two variables without using a third variable and print the swapped values.

## ALGORITHM :
1. Start the program.
2. Import the `Scanner` class to read input from the user.
3. Read the values of two variables `a` and `b`.
4. Print the values before swapping.
5. Use the XOR (`^`) operator to swap the values of `a` and `b` without a third variable.
6. Print the values after swapping.
7. End.

## PROGRAM:
```
/*
Program to swap the values of two variables without using a third variable
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 1E_SWAP_VALUES_WITHOUT_THIRD_VARIABLE.JAVA:
```java
import java.util.*;

public class main {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        
        System.out.printf("Before swapping: a = %d, b = %d", a, b);
        System.out.println();
        
        a = a ^ b;
        b = a ^ b;
        a = a ^ b;
        
        System.out.printf("After swapping: a = %d, b = %d", a, b);
        System.out.println();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/1aeaefae-c567-41e3-bd08-3d86a8923a5d)


## RESULT:
Thus, the Java program to swap the values of two variables without using a third variable was implemented and executed successfully.
