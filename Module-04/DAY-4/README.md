# Ex.No:4(D) COMPANY CLASS WITH FINAL VARIABLES

## AIM:
To create a `final` class `Company` with a `final` variable `companyId`, and member variables for `companyName` and `address`. The program will display the company's details by calling the `print()` method.

## ALGORITHM:
1. Create a `final` class `Company`.
2. Declare a `final` variable `companyId` with the value "ED12G45".
3. Declare member variables for `companyName` and `address`.
4. Initialize these member variables through the constructor.
5. Define the `print()` method to display the details of the company.
6. In the `Main` class, create an instance of `Company` and call the `print()` method to display the company's details.

## PROGRAM:
```
Developed by: Ragul S
RegisterNumber: 212222060184

```
### 4D_COMPANY_CLASS.JAVA:
```java
final class Company {
    final String companyId = "ED12G45";
    String companyName;
    String address;

    Company(String companyName, String address) {
        this.companyName = companyName;
        this.address = address;
    }

    void print() {
        System.out.println("Company Details are,");
        System.out.println("Id is " + companyId);
        System.out.println("Name is " + companyName);
        System.out.println("Address is " + address);
    }
}

public class Main {
    public static void main(String[] args) {
        Company company = new Company("ABC Foods", "Chennai");
        company.print();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/cd68c8d0-87ee-461b-9526-81deb28a10d0)


## RESULT:
The Java program successfully demonstrates the use of a `final` class and `final` variable. The output displays the company's details, and the `companyId` is immutable since it is declared `final`.
