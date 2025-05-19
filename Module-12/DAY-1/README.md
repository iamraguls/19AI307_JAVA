# Ex.No:12(A) TREE MAP SEARCH

## AIM:
To create a Java program to search a key in a TreeMap.

## ALGORITHM:
1. Start the program.
2. Create a TreeMap to store string keys and values.
3. Read the number of entries from the user.
4. Insert the key-value pairs into the TreeMap.
5. Display the TreeMap.
6. Check whether the TreeMap contains the keys "C1" and "C5".
7. Display appropriate messages.
8. End.

## PROGRAM:
```
/*
Program to search a key in a TreeMap using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11F_TREE_MAP_SEARCH.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        TreeMap<String, String> map = new TreeMap<>();
        for (int i = 0; i < n; i++) {
            String key = sc.next();
            String value = sc.next();
            map.put(key, value);
        }
        System.out.println(map);
        if (map.containsKey("C1")) System.out.println("The Tree Map contains key C1");
        if (map.containsKey("C5")) {
            System.out.println("The Tree Map contains key C5");
        } else {
            System.out.println("The TreeMap does not contain key C5");
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/127d1d08-a85f-4992-8b2e-3e197aae7f03)



## RESULT:
Thus, the Java program to search a key in a TreeMap has been implemented and executed successfully.
