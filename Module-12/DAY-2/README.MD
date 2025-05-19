# Ex.No:12(B) COMPARATOR USING SEPARATE CLASS

## AIM:
To create a Java program to illustrate Comparator using a separate class (PercentageComparator) and display the students in descending order of percentage.

## ALGORITHM:
1. Start the program.
2. Create a `Student` class with name and percentage attributes.
3. Create a `PercentageComparator` class that implements `Comparator<Student>`.
4. In the `compare` method, compare students by percentage in descending order.
5. In the main class, read student data from the user and add it to a list.
6. Sort the list using `Collections.sort()` with the comparator.
7. Display the sorted list.
8. End.

## PROGRAM:
```
/*
Program to implement Comparator using Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 11G_COMPARATOR_JAVA:
```java
import java.util.*;

class Student {
    String name;
    double percentage;

    Student(String name, double percentage) {
        this.name = name;
        this.percentage = percentage;
    }
}

class PercentageComparator implements Comparator<Student> {
    public int compare(Student s1, Student s2) {
        return Double.compare(s2.percentage, s1.percentage);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        List<Student> list = new ArrayList<>();
        for (int i = 0; i < n; i++) {
            String name = sc.next();
            double percentage = sc.nextDouble();
            list.add(new Student(name, percentage));
        }

        Collections.sort(list, new PercentageComparator());

        System.out.println("Avg % --> Name");
        System.out.println("---------------------");
        for (Student s : list) {
            System.out.println(s.percentage + " --> " + s.name);
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/35ee7d86-cf07-41ee-a228-ae9a8c4e7432)



## RESULT:
Thus, the Java program illustrating `Comparator` using a separate class to sort students by percentage in descending order was implemented successfully.
