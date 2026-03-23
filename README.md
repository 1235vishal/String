# Java String & StringBuilder Practice 🚀

This file contains basic Java programs demonstrating:

* String immutability
* String methods (`length`, `charAt`, `substring`, etc.)
* String comparison
* String reverse
* Palindrome check
* StringBuilder usage

---

## 🔹 Complete Code

```java
class Main {
    public static void main(String[] args) {

        // ===============================
        // 🔹 STRING BASICS
        // ===============================

        // String s = "Hello";
        // s = s + " world";
        // System.out.println(s);

        // System.out.println("String is immutable in Java (cannot be changed)");

        // String Name = new String("vishal");
        // System.out.println(Name);

        // ===============================
        // 🔹 STRING METHODS
        // ===============================

        // String s = "Hello world";
        // System.out.println("Length: " + s.length());
        // System.out.println("First char: " + s.charAt(0));
        // System.out.println("Substring: " + s.substring(0, 5));

        // ===============================
        // 🔹 STRING COMPARISON
        // ===============================

        // String a = "Hii";
        // String b = "Hiii";

        // System.out.println(a.equals(b));     // true/false
        // System.out.println(a.compareTo(b));  // 0, -1, +1

        // ===============================
        // 🔹 SEARCH & CASE METHODS
        // ===============================

        // System.out.println(s.contains("wo")); // true/false

        // String upper = s.toUpperCase();
        // String lower = s.toLowerCase();

        // System.out.println(upper);
        // System.out.println(lower);

        // ===============================
        // 🔹 SUBSTRING MODIFICATION
        // ===============================

        String name = "vishal rajput";

        // String p1 = name.substring(0,1);
        // String p2 = name.substring(0,6).toUpperCase();
        // String p3 = name.substring(6);

        // String result = p2 + p3;
        // System.out.println(result); 
        // Output: VISHAL rajput

        // ===============================
        // 🔹 LOOP THROUGH STRING
        // ===============================

        for(int i = 0; i < name.length(); i++) {
            // System.out.print(name.charAt(i));
        }

        // ===============================
        // 🔹 STRING REVERSE (Manual)
        // ===============================

        String Name = "isha rajput";
        String rev = "";

        for(int i = Name.length() - 1; i >= 0; i--) {
            rev += Name.charAt(i);
        }

        // System.out.println(rev);

        // ===============================
        // 🔹 STRINGBUILDER OPERATIONS
        // ===============================

        /*
        StringBuilder sb = new StringBuilder("Hello");

        sb.append(" world");
        System.out.println(sb);

        sb.insert(5, " java");
        System.out.println(sb);

        sb.delete(6, 10);
        System.out.println(sb);

        sb.reverse();
        System.out.println(sb);

        System.out.println(sb.charAt(1));

        sb.setCharAt(0, 'V');
        System.out.println(sb);

        System.out.println(sb.length());

        sb.reverse();
        String str = sb.toString();
        System.out.println(str);
        */

        // ===============================
        // 🔹 STRINGBUILDER LOOP APPEND
        // ===============================

        StringBuilder sb = new StringBuilder();

        for(int i = 0; i < 5; i++) {
            sb.append(i);
        }

        System.out.println(sb.toString());

        // ===============================
        // 🔹 REVERSE USING STRINGBUILDER
        // ===============================

        String s = "hello";
        String Rev = new StringBuilder(s).reverse().toString();

        System.out.println(Rev);

        // ===============================
        // 🔹 PALINDROME CHECK
        // ===============================

        String sv = "madam";
        String r1 = new StringBuilder(sv).reverse().toString();

        if(sv.equals(r1)) {
            System.out.println("Palindrome");
        } else {
            System.out.println("Not Palindrome");
        }
    }
}
```

---

## 🔹 Key Concepts

* **String is immutable** → cannot be changed
* **StringBuilder is mutable** → faster for modifications
* Use `equals()` for comparison (not `==`)
* `StringBuilder` is best for:

  * Reverse
  * Loop concatenation
  * Large string operations

---

## 🔹 Output Example

```
01234
olleh
Palindrome
```

---

## 📌 Tip

👉 Prefer `StringBuilder` over `String` in loops to avoid performance issues.

---
