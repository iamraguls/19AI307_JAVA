# Ex.No:6(A) Regular Inner Class Implementation

## AIM:
To implement a regular inner class concept in Java, which involves creating an inner class inside another class to display student details and marks.

## ALGORITHM:
1. Create the outer class `Progress_Report` which contains private members `Stu_Id` and `Password`.
2. Inside the outer class, create an inner class `Exam` with private members `mark1`, `mark2`, and `mark3`.
3. Define a method `display()` in the inner class to calculate and display the total marks and student details.
4. In the `main()` method, instantiate the outer class object and then instantiate the inner class object.
5. Call the `display()` method of the inner class to display the results.

## PROGRAM:
```
/*
Program to implement Regular Inner Class to display student details and marks.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6A_REGULAR_INNER_CLASS.JAVA:
```java
class Progress_Report {
    private String Stu_Id;
    private String Password;

    Progress_Report(String Stu_Id, String Password) {
        this.Stu_Id = Stu_Id;
        this.Password = Password;
    }

    class Exam {
        private float mark1, mark2, mark3;

        Exam(float mark1, float mark2, float mark3) {
            this.mark1 = mark1;
            this.mark2 = mark2;
            this.mark3 = mark3;
        }

        public void display() {
            float total = mark1 + mark2 + mark3;
            System.out.println(Stu_Id + " " + Password + " " + total);
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Progress_Report report = new Progress_Report("User12345", "Student_1");
        Progress_Report.Exam exam = report.new Exam(89, 78, 67);
        exam.display();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/f75ac631-b88e-45a0-8103-6333a6c140c1)



## RESULT:
The Java program was successfully implemented using a regular inner class. The program displayed the student details (Username, Password) along with the total marks calculated from the three subjects.
