# Ex.No:6(D) PACKAGES

## AIM:
To create a Java Program for accessing a package from another package using the package name.

## ALGORITHM:
1. Start the Program.
2. Create a directory named `pack` and save `A.java` inside it.
3. Compile `A.java` from the parent directory using `javac pack/A.java`.
4. Create another directory named `mypack` and save `B.java` inside it.
5. Compile `B.java` from the parent directory using `javac mypack/B.java`.
6. Run `B` from the parent directory with `java mypack.B`.

## PROGRAM:
```
/*
Program to implement Packages using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6D_PACKAGES.JAVA:

### A.java (inside the `pack` directory):
```java
package pack;

public class A {
    public void display() {
        System.out.println("This is class A from the pack package.");
    }
}
```

### B.java (inside the `mypack` directory):
```java
package mypack;

import pack.A;

public class B {
    public static void main(String[] args) {
        A obj = new A();
        obj.display();
        System.out.println("This is class B from the mypack package.");
    }
}
```

## OUTPUT:

```
This is class A from the pack package.
This is class B from the mypack package.
```

## RESULT:
Thus, the program has accessed the package from another package successfully.
