# Substring in Java

## What is a Substring?

A substring is a part of a string extracted from an existing string.

Java provides the `substring()` method to extract a portion of a string.

---

## Syntax

### Method 1

```java
string.substring(beginIndex)
```

Returns the substring from `beginIndex` to the end of the string.

### Method 2

```java
string.substring(beginIndex, endIndex)
```

Returns the substring from `beginIndex` to `endIndex - 1`.

---

## Example 1

```java
import java.util.*;
class Main{
    public static String substring(String str, int si, int ei ){
        String substr = "";
        for(int i =si; i<ei; i++){
           substr += str.charAt(i);
        }
        return substr;
    }
public static void main(String args[]){
    
    String str = "raghuram";
    System.out.println(substring(str , 0, 5));
}
}
```

### Output

```text
gramming
```

---

## Example 2

```java
public class SubstringExample {
    public static void main(String[] args) {

        String str = "Programming";

        System.out.println(str.substring(0, 4));
    }
}
```

### Output

```text
Prog
```

---

## Example 3

```java
public class SubstringExample {
    public static void main(String[] args) {

        String str = "Shubham";

        String result = str.substring(0, 4);

        System.out.println(result);
    }
}
```

### Output

```text
Shub
```

---

## Dry Run

String:

```text
JavaProgramming
```

Index:

```text
J  a  v  a  P  r  o  g  r  a  m  m  i  n  g
0  1  2  3  4  5  6  7  8  9  10 11 12 13 14
```

Code:

```java
str.substring(4, 11);
```

Output:

```text
Program
```

---

## Time Complexity

| Operation             | Time Complexity |
| --------------------- | --------------- |
| substring(start)      | O(n)            |
| substring(start, end) | O(n)            |

Where **n** is the length of the extracted substring.

---

## Space Complexity

```text
O(n)
```

Because a new string is created.

---

## Applications

* Extracting usernames from emails
* Data parsing
* Search operations
* String manipulation
* Text processing

### Example

```java
String email = "shubham@gmail.com";

System.out.println(
    email.substring(0, email.indexOf("@"))
);
```

### Output

```text
shubham
```

---

## Key Points

* `substring()` extracts part of a string.
* Index starts from 0.
* End index is excluded.
* Original string remains unchanged.
* Returns a new string.

## Conclusion

The `substring()` method is one of the most commonly used string operations in Java. It allows developers to extract specific portions of text efficiently for data processing and manipulation.
