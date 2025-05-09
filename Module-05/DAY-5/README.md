# Ex.No:5(E) PALINDROME CHECK USING RECURSION AND HAS-A RELATIONSHIP

## AIM:
To write a Java program to check if a given string is a palindrome or not using recursion and has-a relationship concepts.

## ALGORITHM :
1. Start the program.
2. Define a class `Palindrome` with a method `isPalindrome(String str, int start, int end)` that uses recursion to check if the string is a palindrome.
3. In the `main` class, create an instance of the `Palindrome` class (has-a relationship).
4. Read the input string from the user.
5. Call the `isPalindrome()` method using the object and store the result.
6. Display whether the string is a palindrome or not.
7. End.

## PROGRAM:
```
/*
Program to check if the given string is a palindrome using recursion and has-a relationship in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 5E_PALINDROME_RECURSION_HAS_A.JAVA:
```java
import java.util.*;

class Palindrome{
    public boolean isPalindrome(String str, int start, int end) {
        if (start >= end) {
            return true;
        }
        if (str.charAt(start) != str.charAt(end)) {
            return false;
        }
        return isPalindrome(str, start + 1, end - 1);
    }
}

public class Main{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String str = sc.nextLine();

        Palindrome checker = new Palindrome();
        if (checker.isPalindrome(str, 0, str.length() - 1)) {
            System.out.println(str + " is a palindrome");
        } else {
            System.out.println(str + " is not a palindrome");
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/adb0209d-ccda-43eb-9af9-08379ffd3cbb)


## RESULT:
Thus, the Java program to check if the given string is a palindrome using recursion and has-a relationship was successfully implemented and executed.
