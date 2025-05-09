# Ex.No:2(E) USING PRIVATE ACCESS MODIFIER TO DISPLAY EVEN NUMBERS FROM 0 TO 20

## AIM:
To write a Java program using the private access modifier to display even numbers from 0 to 20.

## ALGORITHM :
1. Start the program.
2. Define a `Main` class with a private static method `display()` that prints even numbers from 0 to 20.
3. In the `main` method, create an object of the `Main` class.
4. Call the `display()` method using the object.
5. End.

## PROGRAM:
```
/*
Program to display even numbers from 0 to 20 using private access modifier in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 2E_PRIVATE_ACCESS_MODIFIER_EVEN_NUMBERS.JAVA:
```java
public class Main {
    private static void display(){
        for(int i = 0; i <= 20; i = i + 2){
            System.out.println(i);
        }
    }

    public static void main(String[] args){
        Main obj = new Main();
        obj.display();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/b2d614e7-dee6-4671-a258-641dab5e48e0)



## RESULT:
Thus, the Java program using the private access modifier to display even numbers from 0 to 20 was implemented and executed successfully.
