
# String in Java

## What is a String?

A String is a sequence of characters used to store and manipulate text data. In Java, strings are represented by the `String` class.

### Examples

```java
String name = "Shubham";
String city = "Varanasi";
String message = "Hello World";
```

---

## Why Do We Use Strings?

Strings are used to store:

* Names
* Addresses
* Messages
* Email IDs
* Passwords
* User Input

Example:

```java
String username = "ShubhamYadav";
```

---

## Creating a String

### Method 1: String Literal

```java
String name = "Shubham";
```

### Method 2: Using new Keyword

```java
String name = new String("Shubham");
```

---

## Common String Methods

### Length

```java
String text = "Java";

System.out.println(text.length());
```

Output:

```text
4
```

### Convert to Uppercase

```java
String text = "java";

System.out.println(text.toUpperCase());
```

Output:

```text
JAVA
```

### Convert to Lowercase

```java
String text = "JAVA";

System.out.println(text.toLowerCase());
```

Output:

```text
java
```

### Access Character

```java
String text = "Java";

System.out.println(text.charAt(0));
```

Output:

```text
J
```

### Compare Strings

```java
String s1 = "Java";
String s2 = "Java";

System.out.println(s1.equals(s2));
```

Output:

```text
true
```

---

## String Concatenation

```java
String firstName = "Shubham";
String lastName = "Yadav";

String fullName = firstName + " " + lastName;

System.out.println(fullName);
```

Output:

```text
Shubham Yadav
```

---

## Example Program

```java
public class StringExample {

    public static void main(String[] args) {

        String name = "Shubham";

        System.out.println("Name: " + name);
        System.out.println("Length: " + name.length());
        System.out.println("Uppercase: " + name.toUpperCase());
    }
}
```

Output:

```text
Name: Shubham
Length: 7
Uppercase: SHUBHAM
```

---

## Time Complexity

| Operation   | Time Complexity |
| ----------- | --------------- |
| length()    | O(1)            |
| charAt()    | O(1)            |
| equals()    | O(n)            |
| substring() | O(n)            |
| concat()    | O(n)            |

Where **n** is the length of the string.

---

## Advantages of Strings

* Easy to store text data
* Built-in methods available
* Secure and immutable
* Widely used in applications

---

## Applications

* User Authentication
* Search Engines
* Chat Applications
* Data Processing
* Web Development

---

## Conclusion

A String is one of the most important data types in Java used to store and manipulate text. Java provides many built-in methods that make string handling efficient and easy.
