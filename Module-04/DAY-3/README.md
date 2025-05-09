# Ex.No:4(C) ANIMAL AND DOG CLASS WITH METHOD OVERRIDING

## AIM:
To demonstrate the concept of method overriding in Java by creating an `Animal` class with a method `display()`, and a child class `Dog` that overrides the `display()` method and calls both overridden and overriding methods using `print()`.

## ALGORITHM:
1. Create a class `Animal` with a method `display()` that prints "I am an Animal".
2. Create a child class `Dog` that inherits from `Animal`.
3. Override the `display()` method in the `Dog` class to print "I am a Dog".
4. Create a new method `print()` in the `Dog` class that calls both the overridden `display()` method and the inherited `display()` method using `super`.
5. In the `main()` method, create an object of `Dog` class and invoke the `print()` method.

## PROGRAM:

### 4C_ANIMAL_DOG_CLASS.JAVA:
```
Developed by: Ragul S
RegisterNumber: 212222060184

```
```java
class Animal {
    void display() {
        System.out.println("I am an animal");
    }
}

class Dog extends Animal {
    @Override
    void display() {
        System.out.println("I am a dog");
    }

    void print() {
        display();
        super.display();
    }
}

public class Main {
    public static void main(String[] args) {
        Dog d = new Dog();
        d.print();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/e1f6c333-b892-4e10-ab8d-364105338cfe)


## RESULT:
The Java program demonstrates method overriding and invocation of both the overridden and overriding methods. The output matches the expected result where the `Dog` class calls both the `display()` method from the `Dog` class and the `display()` method from the `Animal` class using `super`.
