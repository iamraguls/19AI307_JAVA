# Ex.No:6(C) PROGRAM TO DEMONSTRATE CONSTRUCTORS IN INHERITANCE

## AIM:
To create a program demonstrating the use of constructors in inheritance. The program will:
1. Display a message in the parent class constructor.
2. Call the parent class constructor from child class constructors.
3. Display the message for each derived class.

## ALGORITHM :
1. Define the `Animal` class with a constructor that displays "Animal is the Base Class".
2. Define the `Dog` class which extends `Animal` and in its constructor, call the parent constructor using `super()`, then display "Dog is the Derived Class of Animal".
3. Define the `Cat` class which extends `Animal` and in its constructor, call the parent constructor using `super()`, then display "Cat is the Derived Class of Animal".
4. In the `Main` class, create objects of `Dog` and `Cat` to see the constructor behavior.
5. End.

## PROGRAM:
```
/*
Program to demonstrate constructors in inheritance in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6C_INHERITANCE_CONSTRUCTORS.JAVA:
```java
class Animal {
    Animal() {
        System.out.println("Animal is the Base Class");
    }
}

class Dog extends Animal {
    Dog() {
        super();
        System.out.println("Dog is the Derived Class of Animal");
    }
}

class Cat extends Animal {
    Cat() {
        super();
        System.out.println("Cat is the Derived Class of Animal");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog();
        
        Cat cat = new Cat();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/08dfb95d-f675-4a3c-ae4f-556c97572cf3)


## RESULT:
Thus, the Java program demonstrating constructors in inheritance, with parent class constructor being called from child class constructors, was successfully implemented and executed.
