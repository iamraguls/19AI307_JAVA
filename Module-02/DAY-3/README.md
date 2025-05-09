# Ex.No:2(C) DECLARING AND INITIALIZING VALUES INTO AN ARRAY

## AIM:
To declare and initialize values into a one-dimensional array and display the array elements.

## ALGORITHM :
1. Start the program.
2. Declare an integer array and initialize it with values 10, 20, 30, 40, and 50.
3. Print a message "One dimensional array elements are :".
4. Use a `for` loop to iterate through the array and print each element.
5. End.

## PROGRAM:
```
/*
Program to declare, initialize values into an array, and display array elements in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 2C_DECLARE_INITIALIZE_ARRAY.JAVA:
```java
public class ArrayExample {
    public static void main(String[] args) {
        int[] a = {10, 20, 30, 40, 50};
        System.out.println("One dimensional array elements are :");
        System.out.println();
        for (int i = 0; i < a.length; i++) {
            System.out.println("a[" + i + "]:" + a[i]);
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/d0854a2a-fcbc-4ca5-8166-45cc79e4ff33)


## RESULT:
Thus, the Java program to declare and initialize values into a one-dimensional array and display the array elements was implemented and executed successfully.
