# Ex.No:10(B) CREATE LINKEDLIST AND DISPLAY ELEMENTS USING TOARRAY()

## AIM:
To create a LinkedList, read the size of the list, read elements for the LinkedList, and display the elements. Also, apply the `toArray()` method in Java Collection Concepts.

## ALGORITHM :
1. Import the `LinkedList` and `Scanner` classes from the Java library.
2. Create a `LinkedList` of type `Integer`.
3. Read the size of the list from the user.
4. Read elements for the LinkedList and add them using the `add()` method.
5. Display the LinkedList using `System.out.println()`.
6. Convert the LinkedList to an array using the `toArray()` method.
7. Display the array elements.
8. End.

## PROGRAM:
```
/*
Program to create a LinkedList, read elements, and display them using the toArray() method.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 10B_CREATE_LINKEDLIST.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        LinkedList<Integer> list = new LinkedList<>();
        int n = sc.nextInt();
        for (int i = 0; i < n; i++) {
            list.add(sc.nextInt());
        }
        System.out.println("LinkedList: " + list);
        Integer[] array = new Integer[list.size()];
        array = list.toArray(array);
        System.out.print("After converted LinkedList to Array: ");
        for (int i : array) {
            System.out.print(i + " ");
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/e1a0241a-1e52-42e3-b50c-772a99b9fb8d)


## RESULT:
Thus, the Java program to create a LinkedList, read elements, and display them using the `toArray()` method was implemented and executed successfully.
