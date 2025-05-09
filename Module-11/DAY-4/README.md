# Ex.No:11(D) MAP INTERFACE WITH COMPARINGBYVALUE IN DESCENDING ORDER

## AIM:
To create a Java program to demonstrate the `Map` interface, and use `comparingByValue()` to sort the map by value in descending order, and display the key-value pairs.

## ALGORITHM :
1. Start the program.
2. Import necessary classes: `HashMap`, `Map`, `Comparator`, and `Scanner`.
3. Read the size of the map from user input.
4. Use a loop to read key-value pairs and store them in the map.
5. Convert the map into a stream using the `entrySet()` method.
6. Use `comparingByValue()` in descending order to sort the map based on values.
7. Use `forEach()` to display the sorted key-value pairs.
8. End.

## PROGRAM:
```
/*
Program to demonstrate Map interface and sorting by value in descending order using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11D_MAP_INTERFACE_COMPARINGBYVALUE_DESCENDING.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Map<Integer, String> map = new HashMap<>();
        Scanner sc = new Scanner(System.in);
        int size = sc.nextInt();
        for (int i = 0; i < size; i++) {
            int key = sc.nextInt();
            String value = sc.next();
            map.put(key, value);
        }
        map.entrySet()
           .stream()
           .sorted(Map.Entry.comparingByValue(Comparator.reverseOrder()))
           .forEach(entry -> System.out.println(entry.getKey() + "=" + entry.getValue()));
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/d79d540e-5a4a-475c-be5d-df93911fa395)




## RESULT:
Thus, the Java program to demonstrate the `Map` interface and sort key-value pairs by value in descending order using `comparingByValue()` was successfully implemented and executed.
