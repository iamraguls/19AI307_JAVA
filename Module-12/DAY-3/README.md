# Ex.No:12(C) VECTOR IMPLEMENTATION IN JAVA COLLECTION

## AIM:
To write a Java program to read and print the elements using `Vector` in Java Collection Framework.

## ALGORITHM :
1. Start the program.
2. Import the required classes: `Scanner` and `Vector`.
3. Create a `Vector` object to store elements.
4. Read the initial size of the vector.
5. Loop to read elements (either string or integer) and add them using `add()` method.
6. Display the current vector.
7. Read the number of new elements to be added.
8. Loop again to read and add the new elements.
9. Display the updated vector.
10. End.

## PROGRAM:
```
/*
Program to implement Vector in Java Collection
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11E_VECTOR_IMPLEMENTATION.JAVA:
```java
import java.util.Scanner;
import java.util.Vector;

public class VectorExample1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Vector<Object> vec = new Vector<>();
        int initialSize = sc.nextInt();
        sc.nextLine();
        for (int i = 0; i < initialSize * 2; i++) {
            String input = sc.nextLine();
            try {
                int num = Integer.parseInt(input);
                vec.add(num);
            } catch (NumberFormatException e) {
                vec.add(input);
            }
        }
        System.out.println("The vector is: " + vec);
        int addSize = sc.nextInt();
        sc.nextLine();
        for (int i = 0; i < addSize; i++) {
            String input = sc.nextLine();
            try {
                int num = Integer.parseInt(input);
                vec.add(num);
            } catch (NumberFormatException e) {
                vec.add(input);
            }
        }
        System.out.println("The new Vector is: " + vec);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/7c11696e-d544-482d-89ab-cb08072a07f7)


## RESULT:
Thus, the Java program to read and print elements using `Vector` in the Collection Framework was successfully implemented and executed.
