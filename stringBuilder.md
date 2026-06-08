# StringBuilder in Java

## What is StringBuilder?

`StringBuilder` is a class in Java used to create and modify strings efficiently.

Unlike `String`, a `StringBuilder` object is **mutable**, which means its content can be changed without creating a new object.

---

## Why Use StringBuilder?

When multiple string modifications are required, `StringBuilder` is faster and more memory-efficient than `String`.

### String Example

```java
String str = "Java";
str = str + " Programming";
```

A new object is created every time.

### StringBuilder Example

```java
StringBuilder sb = new StringBuilder("Java");
sb.append(" Programming");
```

The same object is modified.

---

## Creating a StringBuilder

```java
StringBuilder sb = new StringBuilder();
```

or

```java
StringBuilder sb = new StringBuilder("Hello");
```

---

## Common Methods

### append()

Adds text to the end.

```java
StringBuilder sb = new StringBuilder("Java");

sb.append(" Programming");

System.out.println(sb);
```

### Output

```text
Java Programming
```

---

### insert()

Inserts text at a specified position.

```java
StringBuilder sb = new StringBuilder("Jva");

sb.insert(1, "a");

System.out.println(sb);
```

### Output

```text
Java
```

---

### delete()

Removes characters.

```java
StringBuilder sb = new StringBuilder("Java Programming");

sb.delete(4, 16);

System.out.println(sb);
```

### Output

```text
Java
```

---

### reverse()

Reverses the string.

```java
StringBuilder sb = new StringBuilder("Java");

sb.reverse();

System.out.println(sb);
```

### Output

```text
avaJ
```

---

### replace()

Replaces characters.

```java
StringBuilder sb = new StringBuilder("Java");

sb.replace(0, 4, "Python");

System.out.println(sb);
```

### Output

```text
Python
```

---

## Complete Example

```java
import java.util.*;
class file{
public static void main(String args[]){
StringBuilder  sb = new StringBuilder(" ");
for( char ch = 'a'; ch<= 'z'; ch++){
sb.append(ch);
}

System.out.println(sb);
}
}
```

### Output

```text
Java Programming
gnimmargorP avaJ
```

---

## Time Complexity

| Operation   | Time Complexity |
| ----------- | --------------- |
| append()    | O(1) Average    |
| charAt()    | O(1)            |
| setCharAt() | O(1)            |
| insert()    | O(n)            |
| delete()    | O(n)            |
| replace()   | O(n)            |
| reverse()   | O(n)            |

Where **n** is the length of the string.

---

## Space Complexity

```text
O(n)
```

Where **n** is the number of characters stored.

---

## String vs StringBuilder

| Feature      | String | StringBuilder |
| ------------ | ------ | ------------- |
| Mutable      | No     | Yes           |
| Performance  | Slower | Faster        |
| Memory Usage | More   | Less          |
| Thread Safe  | Yes    | No            |

---

## Applications

* Building large strings
* Competitive Programming
* String Manipulation
* Text Processing
* Reversing Strings
* Generating Dynamic Content

---

## Advantages

* Fast string modification
* Better memory utilization
* Efficient for loops and repeated concatenation
* Rich set of methods

---

## Conclusion

`StringBuilder` is a mutable class in Java designed for efficient string manipulation. It is preferred over `String` when multiple modifications such as append, insert, delete, replace, and reverse operations are required.
