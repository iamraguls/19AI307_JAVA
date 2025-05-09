# Ex.No:10(C) HASHSET CONCEPTS IN COLLECTION

## AIM:
To demonstrate the use of HashSet in Java Collection Framework. We will add elements to a HashSet and then display the elements by iterating using a `while` loop. The elements in a HashSet are stored in an unordered manner.

## ALGORITHM:
1. Import `HashSet`, `Scanner`, and `Iterator` from the Java library.
2. Create a `HashSet` of type `String`.
3. Read the number of elements to be added to the HashSet.
4. Use a `for` loop to read and add the elements to the HashSet.
5. Use an `Iterator` to iterate through the HashSet.
6. Use a `while` loop to print each element using `Iterator`.
7. End.

## PROGRAM:
```
/*
Program to demonstrate HashSet in Collection Framework and iterate using while loop.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 10C_HASHSET.JAVA:
```java
import java.util.*;

public class Main {
  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    // Creating a HashSet to store elements
    HashSet<String> set = new HashSet<>();
    
    // Read number of elements
    int n = sc.nextInt();
    sc.nextLine();  // Consume the leftover newline
    
    // Reading elements from the user
    for (int i = 0; i < n; i++) {
      set.add(sc.nextLine());
    }

    // Iterating and displaying the elements using while loop and Iterator
    Iterator<String> itr = set.iterator();
    while (itr.hasNext()) {
      System.out.println(itr.next());
    }
  }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c8bae57a-e80c-4691-8feb-a183a344bf29)


## RESULT:
Thus, the Java program using HashSet concepts in collection, adding elements, and iterating through the set using a `while` loop was successfully implemented and executed.
