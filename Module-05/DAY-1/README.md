# Ex.No:5(A) APPLY ENCAPSULATION CONCEPTS WITH SETTER AND GETTER METHODS

## AIM:
To apply the concept of encapsulation in Java using a class with a private field and its corresponding setter and getter methods.

## ALGORITHM:
1. Create a class with a private field `name`.
2. Create public methods `getName()` and `setName(String name)` to access and modify the field.
3. Read input from user and set it using the setter method.
4. Display the field using the getter method.

## PROGRAM:

### 5A_ENCAPSULATION.JAVA:

/*
Developed by: Ragul S
RegisterNumber: 212222060184
*/

```java
import java.util.*;

public class College {
    private String name;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String inp = sc.nextLine();
        College new_name = new College();
        new_name.setName(inp);
        System.out.println(new_name.getName());
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/3f48f277-f760-4e53-b29c-5ccd177e3525)


## RESULT:
The Java program successfully demonstrates the use of encapsulation with getter and setter methods to display the name of a person.
