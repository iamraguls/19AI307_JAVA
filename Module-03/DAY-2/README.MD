# Ex.No:3(B) PROGRAM TO CONCATENATE STRINGS IN SHORT+LONG+SHORT ORDER

## AIM:
To write a Java program that returns a string in the form of short+long+short, with the shorter string on the outside and the longer string on the inside.

## ALGORITHM :
1. Start the program.
2. Read two strings, `a` and `b`, from the user input.
3. Define a method `shortLongShort` to check the length of both strings.
4. If the length of string `a` is greater than string `b`, return `b + a + b`.
5. If the length of string `b` is greater than string `a`, return `a + b + a`.
6. Print the result from the method call.
7. End.

## PROGRAM:
```
/*
Program to concatenate strings in short+long+short order in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 3B_SHORT_LONG_SHORT_STRING.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        String b = sc.nextLine();
        System.out.println(shortLongShort(a, b));
    }

    public static String shortLongShort(String a, String b) {
        if (a.length() > b.length()) {
            return b + a + b;
        } else {
            return a + b + a;
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c823278e-4782-4dc4-aae8-729c73549b83)



## RESULT:
Thus, the Java program that concatenates two strings in the short+long+short order was successfully implemented and executed.
