# Ex.No:10(E) SWAPPING ELEMENTS IN A LIST

## AIM:
To write a Java program to swap the first element (index 0) with the third element (index 2) in an `ArrayList`.

## ALGORITHM :
1. Start the program.
2. Import the necessary classes: `ArrayList`, `Collections`, and `Scanner`.
3. Read the number of elements to be added to the `ArrayList`.
4. Use a loop to read and add elements to the list.
5. Print the list before swapping the elements.
6. Use `Collections.swap()` to swap the first and third elements in the list.
7. Print the list after the swap.
8. End.

## PROGRAM:
```
/*
Program to swap two elements in a list using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 10E_SWAP_ELEMENTS_IN_LIST.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();
        ArrayList<String> list = new ArrayList<>();
        for(int i = 0; i < n; i++) {
            list.add(sc.nextLine());
        }

        System.out.println("Array list before Swap:");
        for(String s : list) {
            System.out.println(s);
        }

        Collections.swap(list, 0, 2);

        System.out.println("Array list after swap:");
        for(String s : list) {
            System.out.println(s);
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/aaa40487-5f08-4fca-b047-283e029048b1)



## RESULT:
Thus, the Java program to swap the first and third elements in an `ArrayList` was implemented and executed successfully.
