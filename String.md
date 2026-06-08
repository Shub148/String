# Input String in Java

## Introduction

An input string is a sequence of characters entered by a user or provided within a program. In Java, strings are represented using the `String` class, which is part of the `java.lang` package.

## Declaring a String

```java
String name = "Shubham";
```

## Taking String Input from User

```java
import java.util.*;
class file {
public class static void main(String[] args){
Scanner sc = new Scanner(System.in);
String name;
// name = sc.next();n//print only one word
name = sc.nextLine(); // print whole line
System.out.println(name);

}
}
```

## Common String Methods

### Length of String

```java
String text = "Java";
System.out.println(text.length());
```

### Convert to Uppercase

```java
String text = "java";
System.out.println(text.toUpperCase());
```

### Convert to Lowercase

```java
String text = "JAVA";
System.out.println(text.toLowerCase());
```

### Access Character

```java
String text = "Java";
System.out.println(text.charAt(0));
```

### Check Equality

```java
String s1 = "Java";
String s2 = "Java";

System.out.println(s1.equals(s2));
```

### Find Substring

```java
String text = "Programming";
System.out.println(text.substring(0, 4));
```

## Example Program

```java
import java.util.Scanner;

public class StringExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a string: ");
        String input = sc.nextLine();

        System.out.println("String Entered: " + input);
        System.out.println("Length: " + input.length());
        System.out.println("Uppercase: " + input.toUpperCase());
        System.out.println("Lowercase: " + input.toLowerCase());
    }
}
```

## Applications of Strings

* User name input
* Password validation
* Text processing
* Search functionality
* Data storage and manipulation
* Chat and messaging applications

## Conclusion

Strings are one of the most important data types in Java. They are used to store and manipulate textual data and provide numerous built-in methods for efficient processing.
