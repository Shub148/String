# Palindrome Number in Java

## Problem Statement

Given an integer `x`, return `true` if `x` is a palindrome, and `false` otherwise.

A palindrome number reads the same forward and backward.

## Examples

### Example 1

**Input:**

```text
121
```

**Output:**

```text
true
```

**Explanation:**

```text
121 reversed is 121.
```

---

### Example 2

**Input:**

```text
-121
```

**Output:**

```text
false
```

**Explanation:**

```text
Forward: -121
Backward: 121-
```

They are not the same.

---

### Example 3

**Input:**

```text
10
```

**Output:**

```text
false
```

**Explanation:**

```text
10 reversed is 01.
```

---

## Java Code

```java
import java.util.*;
class file {
public static boolean isPalindrome(String str){
for(int i=0; i<str.length()/2; i++){
int n = str.length();
if(str.charAt(i) != str.charAt(n-1-i){
return false;
}
}
return true;
}
public static void main(String[] args){
String str = "1 2 1";
System.out.println(isPalindrome(str));

}
}
```

---

## Dry Run

### Input

```teimport xt
121
```

### Iteration 1

```text
digit = 1
reverse = 1
x = 12
```

### Iteration 2

```text
digit = 2
reverse = 12
x = 1
```

### Iteration 3

```text
digit = 1
reverse = 121
x = 0
```

### Result

```text
original = 121
reverse = 121
```

Output:

```text
true
```

---

## Time Complexity

```text
O(log10 n)
```

Reason:

* We process each digit of the number once.

---

## Space Complexity

```text
O(1)
```

Reason:

* Only a few variables are used.
* No extra data structures are required.

---

## Key Points

* Negative numbers are never palindromes.
* Reverse the number digit by digit.
* Compare the reversed number with the original number.
* Efficient solution with constant extra space.

## Tags

```text
Math
Palindrome
Number Manipulation
Java
LeetCode 9
```
