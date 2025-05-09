# Ex.No:7(C) THREAD CREATION USING `extends Thread`

## AIM:
To write a Java program to create a thread using the `Thread` class by extending it and display the thread name input by the user.

## ALGORITHM:
1. Start the program.
2. Create a class that extends `Thread`.
3. Inside the `run()` method, get username input using `Scanner` and display the thread name.
4. In `main()`, create an object of the class and start the thread using `start()` method.

## PROGRAM:
```
/*
Program to create Thread using extends Thread class
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 7A_THREAD_EXTENDS.JAVA:
```java
import java.util.*;
public class Multi extends Thread
{  
    Scanner sc=new Scanner(System.in);
    public void run()
    {  
        String sname=sc.nextLine();
        System.out.println("Thread Name:" +sname);  
    }  
    public static void main(String args[]){  
        Multi t1=new Multi();  
        t1.start();  
    }      
}  
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ff67f29e-1b2a-4741-bc03-b5f7c5544499)


## RESULT:
Thus, the Java program to create a thread using `extends Thread` was successfully written and executed.
