# Ex.No:4(A) PARAMETERIZED CONSTRUCTOR IN THE EMPLOYEE CLASS

## AIM:
To create a parameterized constructor in the `Employee` class that initializes the `name` and `dept` fields, and call the `getName()` and `getDept()` methods in the main method of the `Sample` class to print the values.

## ALGORITHM :
1. Define the `Employee` class with fields `name` and `dept`.
2. Create a parameterized constructor in the `Employee` class that initializes the `name` and `dept` with passed values.
3. Create `getName()` and `getDept()` methods to return the `name` and `dept`.
4. In the `Sample` class, create an instance of `Employee` and pass the values "Antony" and "AIML" to the constructor.
5. Call the `getName()` and `getDept()` methods to retrieve the values and print them.
6. End the program.

## PROGRAM:
```
/*
Program to demonstrate parameterized constructor in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 4A_EMPLOYEE_CLASS.JAVA:
```java
class Employee {
    String name;
    String dept;

    public Employee(String name, String dept) {
        this.name = name;
        this.dept = dept;
    }

    public String getName() {
        return name;
    }

    public String getDept() {
        return dept;
    }
}

public class Sample {
    public static void main(String[] args) {
        Employee e = new Employee("Antony", "AIML");

        System.out.println(e.getName());
        System.out.println(e.getDept());
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/2fddf1a1-103a-46fb-8e56-15f823cfa571)


## RESULT:
Thus, the Java program using a parameterized constructor in the `Employee` class to initialize and print the values was successfully implemented and executed.
