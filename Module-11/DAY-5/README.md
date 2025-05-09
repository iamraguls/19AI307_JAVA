# Ex.No:11(E) REMOVE KEY AND DISPLAY FROM `HASHMAP`

## AIM:
To create a Java program to remove a specified key (100) from a `HashMap` and display the remaining key-value pairs, along with the removed value.

## ALGORITHM :
1. Start the program.
2. Import necessary classes: `HashMap` and `Scanner`.
3. Read the size of the map from user input.
4. Use a loop to read key-value pairs and store them in the `HashMap`.
5. Display all key-value pairs using a loop.
6. Use the `remove()` method to remove the key `100` from the map.
7. Print the removed value.
8. End.

## PROGRAM:
```
/*
Program to remove a key from HashMap and display key-value pairs using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11E_REMOVE_KEY_DISPLAY_HASHMAP.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashMap<Integer, String> map = new HashMap<>();
        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            String value = sc.next();
            map.put(key, value);
        }
        for (Map.Entry<Integer, String> entry : map.entrySet()) {
            System.out.println("key: " + entry.getKey() + " value: " + entry.getValue());
        }
        String removed = map.remove(100);
        System.out.println("Following value is removed from Map: " + removed);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/f41a3bc8-83b3-4b77-ae84-223952e1cb74)


## RESULT:
Thus, the Java program to remove a specified key (`100`) from a `HashMap` and display the remaining key-value pairs along with the removed value was successfully implemented and executed.
