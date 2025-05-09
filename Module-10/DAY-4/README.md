# Ex.No:10(D) HASHSET COLLECTION DEMONSTRATION

## AIM:
To demonstrate the usage of `HashSet` in Java by adding elements to it, displaying the elements, and iterating over them while ignoring duplicate entries.

## ALGORITHM :
1. Start the program.
2. Import the `HashSet` class and the `Scanner` class for input.
3. Create a `HashSet` to store unique elements.
4. Read the number of elements to be added.
5. Use a loop to add elements to the `HashSet`.
6. Create an iterator to traverse through the `HashSet`.
7. Use a `while` loop to iterate and display each element.
8. End.

## PROGRAM:
```
/*
Program to demonstrate HashSet collection and iterate while ignoring duplicates using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 10D_HASHSET_COLLECTION.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        HashSet<String> hashSet = new HashSet<>();
        int size = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < size; i++) {
            hashSet.add(sc.nextLine());
        }
        Iterator<String> iterator = hashSet.iterator();
        
        while (iterator.hasNext()) {
            System.out.println(iterator.next());
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/9d9cbd3b-a962-4f7b-8301-801a73f54cf4)


## RESULT:
Thus, the Java program using `HashSet` was implemented and executed successfully to add elements, ignore duplicates, and iterate through the set.
