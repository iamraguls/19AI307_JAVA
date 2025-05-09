# Ex.No:7(D) THREAD CREATION USING SYNCHRONIZATION

## AIM:
To write a Java program to perform multiplication table using synchronized method with two threads.

## ALGORITHM:
1. Create a `Table` class with a `synchronized` method `printTable(int n)` to print multiplication table.
2. Create two thread classes `MyThread1` and `MyThread2`, extend them from `Thread` and override `run()` method.
3. In `run()`, call the `printTable()` method with different values (5 and 100).
4. In `main()`, create a `Table` object and pass it to both threads and start them.

## PROGRAM:
```
/*
Program to perform multiplication using Synchronization
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 7B_THREAD_SYNC.JAVA:
```java
class Table {
    synchronized void printTable(int n) {
        for (int i = 1; i <= 5; i++) {
            System.out.println(n * i);
            try {
                Thread.sleep(400);
            } catch (InterruptedException e) {
                System.out.println(e);
            }
        }
    }
}

class MyThread1 extends Thread {
    Table t;

    MyThread1(Table t) {
        this.t = t;
    }

    public void run() {
        t.printTable(5);
    }
}

class MyThread2 extends Thread {
    Table t;

    MyThread2(Table t) {
        this.t = t;
    }

    public void run() {
        t.printTable(100);
    }
}

public class Main {
    public static void main(String[] args) {
        Table obj = new Table();
        MyThread1 t1 = new MyThread1(obj);
        MyThread2 t2 = new MyThread2(obj);
        t1.start();
        t2.start();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/60bde9d7-d236-4e17-b4d3-b7ac35bd86ee)


## RESULT:
Thus, the Java program using synchronized method and multithreading was successfully written and executed.
