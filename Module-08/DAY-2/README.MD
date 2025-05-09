# Ex.No:8(B) FILE OPERATION - STRINGREADER

## AIM:
To write a Java program to read the content from a string using Reader.

## ALGORITHM:
1. Import `java.io.*` and `java.util.*`.
2. Use `Scanner` to read the input string.
3. Create a `char[]` array of size 12.
4. Use `StringReader` to read characters into the array.
5. Display the data using `System.out.println()`.

## PROGRAM:
```
/*
Program to read content using StringReader
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 8B_STRING_READER.JAVA:
```java
import java.io.*;  
import java.util.*;
public class Main {  
    public static void main(String[] args) {
        try {   
            Scanner sc = new Scanner(System.in);
            String str = sc.nextLine();
            char[] array = new char[12];
            Reader r = new StringReader(str);
            r.read(array);
            System.out.println("Data read from the string:");
            System.out.println(array);
        } catch(Exception e) {
            System.out.println(e);
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/10b3ea51-4b76-4485-a128-8e85b4838c26)


## RESULT:
Thus, the Java program to read content from the string using Reader was successfully written and executed.
