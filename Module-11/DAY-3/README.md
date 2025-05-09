# Ex.No:11(C) CHECKING KEY/VALUE EXISTENCE IN `LINKEDHASHMAP`

## AIM:
To write a Java program to create and add objects to a `LinkedHashMap` and check whether a particular key and value exist.

## ALGORITHM :
1. Start the program.
2. Import necessary classes: `LinkedHashMap` and `Scanner`.
3. Read the size of the map from user input.
4. Use a loop to read key-value pairs and add them to the `LinkedHashMap`.
5. Display the contents of the map by iterating through it.
6. Use the `containsKey()` method to check if a particular key exists in the map.
7. Use the `containsValue()` method to check if a particular value exists in the map.
8. End.

## PROGRAM:
```
/*
Program to check the existence of a key/value in LinkedHashMap using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11C_CHECK_KEY_VALUE_EXISTENCE_IN_LINKEDHASHMAP.JAVA:
```java
import java.util.*;

public class Mapp {
    public static void main(String args[]) {
        LinkedHashMap<Integer, Double> map = new LinkedHashMap<>();
        Scanner sc = new Scanner(System.in);

        int size = sc.nextInt();
        for (int i = 0; i < size; i++) {
            int key = sc.nextInt();
            double value = sc.nextDouble();
            map.put(key, value);
        }

        for (Map.Entry<Integer, Double> entry : map.entrySet()) {
            System.out.println(entry.getKey() + " " + entry.getValue());
        }

        System.out.println(map.containsKey(3));
        System.out.println(map.containsValue(3.3));
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ddfa100d-3063-4d41-964a-f7315d6088f9)




## RESULT:
Thus, the Java program to create and add objects to a `LinkedHashMap` and check for the existence of a particular key and value was successfully implemented and executed.
