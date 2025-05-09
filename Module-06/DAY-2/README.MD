# Ex.No:6(B) INHERITANCE DEMONSTRATION WITH VEHICLE, CAR, AND ALTO CLASSES

## AIM:
To demonstrate inheritance in Java by creating three classes: `Vehicle`, `Car`, and `Alto`, where `Alto` extends `Car` and `Car` extends `Vehicle`. The classes contain methods to display specific messages, and the main class will demonstrate calling these methods using an object of `Alto`.

## ALGORITHM:
1. Create a class `Vehicle` with a method `display()` that prints "Vehicle Class".
2. Create a class `Car` that extends `Vehicle` and contains a method `print()` that prints "Car Class".
3. Create a class `Alto` that extends `Car` and contains a method `show()` that prints "Alto Class".
4. In the `Main` class, create an object of `Alto` and call all three methods (from `Vehicle`, `Car`, and `Alto`).
5. Display the output.

## PROGRAM:

```
/*
Program to demonstrate inheritance with classes Vehicle, Car, and Alto.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6B_INHERITANCE_VEHICLE_CAR_ALTO.JAVA:

```java
class Vehicle {
    void display() {
        System.out.println("Vehicle Class");
    }
}

class Car extends Vehicle {
    void print() {
        System.out.println("Car Class");
    }
}

class Alto extends Car {
    void show() {
        System.out.println("Alto Class");
    }
}

public class Main {
    public static void main(String[] args) {
        Alto obj = new Alto();
        obj.display(); 
        obj.print();   
        obj.show();    
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/a4434365-dc6f-4b97-a53d-1da73c6c4ecc)


## RESULT:
Thus, the inheritance mechanism in Java was successfully demonstrated by creating three classes: `Vehicle`, `Car`, and `Alto`, with `Alto` extending `Car` and `Car` extending `Vehicle`. The methods from all the classes were successfully accessed in the `Main` class using an object of the `Alto` class.
