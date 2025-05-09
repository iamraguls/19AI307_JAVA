# Ex.No:2(B) DEMONSTRATING THE DEFAULT ACCESS MODIFIER IN JAVA

## AIM:
To demonstrate the use of the default access modifier in Java and print the word "default".

## ALGORITHM :
1. Start the program.
2. Define a class named `BaseClass` with a method `display()` having default access modifier.
3. The `display()` method will print the word "default".
4. Define a class named `Main` with the `main` method.
5. In the `main` method, create an object of the `BaseClass`.
6. Call the `display()` method using the object.
7. End.

## PROGRAM:
```
/*
Program to demonstrate the default access modifier in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 2B_DEFAULT_ACCESS_MODIFIER.JAVA:
```java
class BaseClass {
    void display() {
        System.out.println("default");
    }
}

public class Main {
    public static void main(String[] args) {
        BaseClass obj = new BaseClass();
        
        obj.display(); 
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/8993a4a3-a0b6-4570-bc92-8095fcb84a53)




## RESULT:
Thus, the Java program to demonstrate the default access modifier and print the word "default" was implemented and executed successfully.
