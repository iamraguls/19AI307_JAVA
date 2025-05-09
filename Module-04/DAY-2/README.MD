# Ex.No:4(B) EMPLOYEE CLASS CONTAINING ADDRESS OBJECT

## AIM:
To demonstrate a Java program where an `Employee` object contains a `name` and another object `address` with its own fields such as `doorNo`, `street`, and `city`.

## ALGORITHM:
1. Create an `Address` class with fields `doorNo`, `street`, and `city`.
2. Define a parameterized constructor in `Address` to initialize these fields.
3. Create a method in `Address` to return each field.
4. Create an `Employee` class with a field `name` and an `Address` object.
5. Define a constructor in `Employee` to initialize the `name` and `address`.
6. In the `main` method, create an `Address` object and an `Employee` object using the `Address` object.
7. Print the `name` and address information (using methods of both `Employee` and `Address`).
8. End the program.

## PROGRAM:
```
/*
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

### 4B_EMPLOYEE_WITH_ADDRESS.JAVA:
```java
class Address {
    private String doorNo;
    private String street;
    private String city;

    public Address(String doorNo, String street, String city) {
        this.doorNo = doorNo;
        this.street = street;
        this.city = city;
    }

    public String getDoorNo() {
        return doorNo;
    }

    public String getStreet() {
        return street;
    }

    public String getCity() {
        return city;
    }
}

class Employee {
    private String name;
    private Address address;

    Employee(String name, Address address) {
        this.name = name;
        this.address = address;
    }

    public String getName() {
        return name;
    }

    public Address getAddress() {
        return address;
    }
}

public class Main {
    public static void main(String[] args) {
        Address addr = new Address("10", "100 Feet Road", "Chennai");
        Employee emp = new Employee("Leo", addr);

        System.out.println(emp.getName());
        System.out.println(addr.getDoorNo() + "," + addr.getStreet() + "," + addr.getCity());
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5dcdf2a6-a8aa-4ae6-b401-12abe2ab0333)


## RESULT:
The Java program successfully demonstrates the `Employee` object containing a member `name` and an `address` object, which contains its own information such as `doorNo`, `street`, and `city`. The program executes as expected.
