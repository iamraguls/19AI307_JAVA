# Ex.No:4(E) PARAMETERIZED CONSTRUCTOR IN EMPLOYEE CLASS

## AIM:
To create a parameterized constructor in the `Employee` class that initializes the `name` and `designation` fields with the values "John" and "Asst.Manager", and then prints these values using the `getName()` and `getDesg()` methods.

## ALGORITHM:
1. Create the `Employee` class with member variables `name` and `desg`.
2. Define a parameterized constructor to initialize `name` and `desg` with given values.
3. Define methods `getName()` and `getDesg()` to retrieve the values of `name` and `desg`.
4. In the `Sample` class, create an `Employee` object and call the `getName()` and `getDesg()` methods to print the values.

## PROGRAM:

### 4E_EMPLOYEE_CLASS.JAVA:
```
/*
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```
```java
class Employee {
    String name;
    String desg;

    Employee(String name, String desg) {
        this.name = name;
        this.desg = desg;
    }

    public String getName() {
        return name;
    }

    public String getDesg() {
        return desg;
    }
}

public class Sample {
    public static void main(String[] args) {
        Employee emp = new Employee("John", "Asst.Manager");
        System.out.println(emp.getName());
        System.out.println(emp.getDesg());
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/784ce90d-a3c5-4490-b673-3e4ca9f036ea)


## RESULT:
The Java program successfully demonstrates the use of a parameterized constructor in the `Employee` class. The values "John" and "Asst.Manager" are passed to the constructor, and the `getName()` and `getDesg()` methods correctly print the values.
