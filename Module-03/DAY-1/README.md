# Ex.No:3(A) PROGRAM TO READ INPUT AND SPLIT WORDS FROM A SENTENCE

## AIM:
To write a Java program to read a sentence as input and split the words from the sentence.

## ALGORITHM :
1. Start the program.
2. Read the input sentence using `Scanner`.
3. Split the sentence into words using the `split()` method.
4. Print each word on a new line using a loop.
5. End.

## PROGRAM:
```
/*
Program to read input and split words from a sentence in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 3A_SPLIT_WORDS_FROM_SENTENCE.JAVA:
```java
import java.util.Scanner;

public class SplitWords {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String s = scanner.nextLine();
        String[] words = s.split(" ");
        for (String word : words) {
            System.out.println(word);
        }
        scanner.close();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/505330bd-2270-4adc-a96a-6be312d28247)



## RESULT:
Thus, the Java program to read input and split words from a sentence was implemented and executed successfully.
