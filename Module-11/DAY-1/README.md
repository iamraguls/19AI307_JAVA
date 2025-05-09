# Ex.No:11(A) ADD ELEMENTS OF ONE TREESET TO ANOTHER

## AIM:
To write a Java program to add all the elements of one `TreeSet` to another `TreeSet`.

## ALGORITHM :
1. Start the program.
2. Import the `TreeSet` and `Scanner` classes.
3. Read the size of two `TreeSet` objects.
4. Use a loop to add elements to both `TreeSet` objects.
5. Display both `TreeSet` objects before performing the addition.
6. Use `addAll()` to add all elements from the second `TreeSet` to the first `TreeSet`.
7. Display the updated `TreeSet` after addition.
8. End.

## PROGRAM:
```
/*
Program to add all elements from one TreeSet to another using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11A_ADD_ELEMENTS_TO_TREESET.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int size1 = sc.nextInt();
        int size2 = sc.nextInt();
        
        TreeSet<Integer> treeSet1 = new TreeSet<>();
        for (int i = 0; i < size1; i++) {
            treeSet1.add(sc.nextInt());
        }

        TreeSet<Integer> treeSet2 = new TreeSet<>();
        for (int i = 0; i < size2; i++) {
            treeSet2.add(sc.nextInt());
        }

        System.out.println("Tree set1: " + treeSet1);
        System.out.println("Tree set2: " + treeSet2);

        treeSet1.addAll(treeSet2);
        System.out.println("Tree set1: " + treeSet1);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/845881c7-3d01-4504-b709-aa4d0ac3a027)


## RESULT:
Thus, the Java program to add all elements from one `TreeSet` to another was implemented and executed successfully.
