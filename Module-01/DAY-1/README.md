# Ex.No:1(A) CLASS & OBJECTS – FRUIT CLASS

## AIM:
To create a class named 'Fruit' with variables 'name', 'color', and 'weight' and display the attributes using objects.

## ALGORITHM :
1. Start the program.
2. Define a class named 'Fruit'.
3. Declare variables 'name', 'color' (String), and 'weight' (double).
4. Define a class named 'Main' with the 'main' method.
5. Create two objects of the 'Fruit' class.
6. Assign values to the variables through each object.
7. Print the values of the attributes for each object.
8. End.

## PROGRAM:
```
/*
Program to implement a class & objects using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 1A_CLASS_AND_OBJECTS.JAVA:
```java
class Fruit {
    String name;
    String color;
    double weight;
}

public class Main {
    public static void main(String[] args){
        Fruit obj1 = new Fruit();
        Fruit obj2 = new Fruit();

        obj1.name = "Grape";
        obj1.color = "Purple";
        obj1.weight = 0.75;

        obj2.name = "Mango";
        obj2.color = "Yellow";
        obj2.weight = 1.50;

        System.out.println("Fruit Name is " + obj1.name + ", weight is " + obj1.weight + "kg and Color is " + obj1.color);
        System.out.println("Fruit Name is " + obj2.name + ", weight is " + obj2.weight + "kg and Color is " + obj2.color);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ae9467c5-a53e-4e87-8dd8-259aae4bc8a2)




## RESULT:
Thus, the Java program to implement a class named 'Fruit' and create objects to access and display its attributes was implemented and executed successfully.
