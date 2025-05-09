# Ex.No:6(E) PROGRAM TO DEMONSTRATE METHOD OVERRIDING

## AIM:
To create a program demonstrating method overriding, where the child class overrides the method of the parent class, and both the overridden and overriding methods are invoked using an object of the child class.

## ALGORITHM :
1. Define a `Parent` class with a method `display()` that prints "Parent Class".
2. Define a `Child` class that extends the `Parent` class and overrides the `display()` method to print "Child Class".
3. Add a `print()` method in the `Child` class that calls both the overridden `display()` method (using `display()`) and the parent class method (using `super.display()`).
4. In the `Main` class, create an instance of the `Child` class and call the `print()` method using the object.
5. End.

## PROGRAM:
```
/*
Program to demonstrate method overriding in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6E_METHOD_OVERRIDING.JAVA:
```java
class Parent {
    void display() {
        System.out.println("Parent Class");
    }
}

class Child extends Parent {
    void display() {
        System.out.println("Child Class");
    }

    void print() {
        display();
        super.display();
    }
}

public class Main {
    public static void main(String[] args) {
        Child obj = new Child();
        obj.print();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/23f26de5-4880-489b-bb9d-b5179e383e3d)


## RESULT:
Thus, the Java program demonstrating method overriding, where the child class overrides the `display()` method of the parent class, and both methods are invoked using the `print()` method, was successfully implemented and executed.
