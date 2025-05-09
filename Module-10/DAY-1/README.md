# Ex.No:10(A) CREATE AND DISPLAY ELEMENTS USING ARRAYLIST

## AIM:
To create an ArrayList, read three elements, and display the elements using the `add()` method in Java.

## ALGORITHM :
1. Import the `ArrayList` and `Scanner` classes from the Java library.
2. Create an ArrayList of type `String`.
3. Use a `Scanner` to read three elements from the user.
4. Add the three elements to the ArrayList using the `add()` method.
5. Display the ArrayList.
6. End.

## PROGRAM:
```
/*
Program to create an ArrayList, read three elements, and display the elements using the add function in ArrayList.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 10A_CREATE_ARRAYLIST.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String args[]) {
        ArrayList<String> list = new ArrayList<>();
        Scanner sc = new Scanner(System.in);
        for (int i = 0; i < 3; i++) {
            list.add(sc.next());
        }
        System.out.println(list);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/0c9fd7c0-0685-41cf-a94c-f2b0a071f741)


## RESULT:
Thus, the Java program to create an ArrayList, read three elements, and display the elements using the `add()` method was implemented and executed successfully.
