# Ex.No:12(D) PRIORITY QUEUE IMPLEMENTATION

## AIM:
To write a Java program to display the added elements from the `PriorityQueue`.

## ALGORITHM :
1. Start the program.
2. Import the required classes.
3. Create a `PriorityQueue` of integers.
4. Read the size of the queue from the user.
5. Use a loop to read integer elements and add them to the priority queue.
6. Display the contents of the queue.
7. End.

## PROGRAM:
```
/*
Program to implement PriorityQueue in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 12A_PRIORITY_QUEUE.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        PriorityQueue<Integer> pq = new PriorityQueue<>();

        int size = sc.nextInt();

        for (int i = 0; i < size; i++) {
            pq.add(sc.nextInt());
        }

        System.out.println("Display the element of Queue:");
        System.out.println(pq);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/b10f6258-ead0-4a2c-8573-0910b5cab4c6)


## RESULT:
Thus, the Java program to display the added elements from the `PriorityQueue` was successfully implemented and executed.
