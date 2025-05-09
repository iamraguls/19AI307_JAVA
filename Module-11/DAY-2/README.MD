# Ex.No:11(B) DISPLAYING `CONTAINSKEY` AND RETRIEVING VALUES FROM `HASHMAP`

## AIM:
To write a Java program that displays the `containsKey` result for the key `104` and retrieves the key-value pairs from a `HashMap` by iterating over it using a loop.

## ALGORITHM :
1. Start the program.
2. Import necessary classes: `HashMap`, `Scanner`, and `Map`.
3. Read the size of the `HashMap`.
4. Use a loop to input key-value pairs and store them in the `HashMap`.
5. Iterate over the `HashMap` using a loop and display each key-value pair.
6. Check if the `HashMap` contains the key `104` using the `containsKey` method.
7. Display the result of `containsKey(104)`.
8. End.

## PROGRAM:
```
/*
Program to check containsKey and retrieve key-value pairs from HashMap using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11B_CONTAINSKEY_AND_RETRIEVE_FROM_HASHMAP.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int size = sc.nextInt();
        HashMap<Integer, String> hashMap = new HashMap<>();

        for (int i = 0; i < size; i++) {
            int key = sc.nextInt();
            sc.nextLine(); 
            String value = sc.nextLine();
            hashMap.put(key, value);
        }

        for (Map.Entry<Integer, String> entry : hashMap.entrySet()) {
            System.out.println("key: " + entry.getKey() + " value: " + entry.getValue());
        }

        System.out.println("Does HashMap contains 104 as key: " + hashMap.containsKey(104));
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/86d00f34-5cce-4229-9b7e-1bf0377f7889)



## RESULT:
Thus, the Java program to display the result of `containsKey` and retrieve key-value pairs from a `HashMap` was implemented and executed successfully.
