# Ex.No:7(E) THREAD CREATION USING RUNNABLE INTERFACE

## AIM:
To write a Java program to create a Thread using the Runnable Interface and get a double value from the user.

## ALGORITHM:
1. Create a class `Multi` that implements the `Runnable` interface.
2. Inside the `run()` method, use `Scanner` to get a double value from the user and print it.
3. In the `main()` method, create a `Thread` object by passing an instance of `Multi` and call `start()`.

## PROGRAM:
```
/*
Program to create Thread using Runnable Interface
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 7A_THREAD_RUNNABLE.JAVA:
```java
import java.util.*;

public class Multi implements Runnable {  
    Scanner sc = new Scanner(System.in);
    public void run() {  
        double count = sc.nextDouble();
        System.out.println("Thread Count: " + count);  
    }  

    public static void main(String args[]) {  
        Multi m1 = new Multi(); 
        Thread t1 = new Thread(m1); 
        t1.start();  
    }  
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/4172e921-a68e-4926-b6e1-281e23d54792)


## RESULT:
Thus, the Java program using Runnable Interface to create a thread and get double input was successfully written and executed.
