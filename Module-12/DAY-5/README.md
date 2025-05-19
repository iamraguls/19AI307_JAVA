# Ex.No:12(E) MAP INTERFACE WITH COMPARINGBYKEY IN DESCENDING ORDER

## AIM:
To write a Java program for the Map interface concept and display the keys and values using `comparingByKey()` in descending order.

## ALGORITHM :
1. Start the program.
2. Import necessary packages.
3. Read the number of elements.
4. Create a `HashMap` to store Integer keys and String values.
5. Add elements to the map using a loop.
6. Use a stream to sort the map entries by key in descending order using `comparingByKey(Comparator.reverseOrder())`.
7. Print each key-value pair.
8. End the program.

## PROGRAM:
```
/*
Program to implement map interface using comparingByKey in descending order
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 12B_MAP_DESCENDING_BY_KEY.JAVA:
```java
import java.util.*;
import java.util.stream.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        Map<Integer, String> map = new HashMap<>();
        for(int i = 0; i < n; i++) {
            int key = sc.nextInt();
            String value = sc.next();
            map.put(key, value);
        }
        map.entrySet()
            .stream()
            .sorted(Map.Entry.comparingByKey(Comparator.reverseOrder()))
            .forEach(e -> System.out.println(e.getKey() + "=" + e.getValue()));
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/73a8540c-1b2f-4466-8c48-f734f7028ded)



## RESULT:
Thus, the Java program using Map interface with `comparingByKey()` in descending order was implemented and executed successfully.
