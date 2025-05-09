# Ex.No:9(D) PERFORMING TRANSIENT IN STUDENT DETAILS

## AIM:
To perform serialization and demonstrate the use of the transient keyword in Java for student details (name, department, roll number).

## ALGORITHM :
1. Create a `Studentinfo` class implementing the `Serializable` interface.
2. Define the instance variables `name`, `dept`, and `rollno` in the `Studentinfo` class.
3. Mark the `dept` and `rollno` variables as `transient` to prevent them from being serialized.
4. Create a constructor to initialize the `name`, `dept`, and `rollno` fields.
5. In the main method, create an object of the `Studentinfo` class and assign values to the fields.
6. Serialize the object into a file named "student.txt".
7. Deserialize the object from the file and display the details to verify the behavior of transient fields.
8. End.

## PROGRAM:
```
/*
Program to perform transient in Student details (name, dept, rollno) and serialize the object in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 9D_TRANSIENT_STUDENT_DETAILS.JAVA:
```java
import java.io.*;

class Studentinfo implements Serializable {
    String name;
    transient String dept;
    transient int rollno;

    Studentinfo(String n, String d, int r) {
        this.name = n;
        this.dept = d;
        this.rollno = r;
    }
}

public class Main {
    public static void main(String[] args) {
        try {
            // Create a Studentinfo object
            Studentinfo student = new Studentinfo("Abhi", "CSE", 101);

            // Serialize the object
            FileOutputStream fos = new FileOutputStream("student.txt");
            ObjectOutputStream oos = new ObjectOutputStream(fos);
            oos.writeObject(student);
            oos.close();
            fos.close();

            // Deserialize the object
            FileInputStream fis = new FileInputStream("student.txt");
            ObjectInputStream ois = new ObjectInputStream(fis);
            Studentinfo deserializedStudent = (Studentinfo) ois.readObject();
            ois.close();
            fis.close();

            // Display the values
            System.out.println("Transient-Student Name: " + deserializedStudent.name);
            System.out.println("Transient-Student Department: " + deserializedStudent.dept);
            System.out.println("Transient-Student RollNo: " + deserializedStudent.rollno);

        } catch (Exception e) {
            System.out.println("Exception: " + e);
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/e761249d-b25a-41f5-984b-04a88ca5ad3f)


## RESULT:
Thus, the Java program to demonstrate the transient keyword in Student details and perform serialization was implemented and executed successfully.
