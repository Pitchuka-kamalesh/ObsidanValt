---
Created: 2024-07-25T14:57:00
Topic: Java Basic
Subtopics: String
tags:
  - 🌱
  - baby
Links:
  - "[[Java]]"
Task:
  - String operations
Modified: 2024-07-25T19:21:00
---


---

# Strings
---

String is a group of characters and it is immutable data type and  it is a object reference how to create a string 

- How to create a string  in two ways 

```java
String name = "JavaHome";

String names = new String(names);

```

- How to find the length of the String 

```java
public class Tester{

	 public static void main(String args[]){
		
		String name = "Hello java";
		System.out.println("Length of the String "+ name.length());
		
	 }
}
```

- how to get the Substring from the string
```java
public class Tester{

	 public static void main(String args[]){
		
		String name = "Hello java";
		// Substring is a part of the string which we want to like  `varibleName.substring();`
		System.out.println("Length of the String "+ name.substring(3,name.length()));
		
		
	 }
}


```

- Concatenation of two Strings  
```java
public class Tester{

	 public static void main(String args[]){
		
		String name = "Hello java";
		String test = "Selenium";
		String concat = name + " "+ test;
		System.out.println(concat);
		
	 }
}
```
- Equality of String 
 there are Two methods  `equals` & `equalIgnoreCase`
  
  Equals method to equals two strings 
  ```java
	  public class Tester{

	 public static void main(String args[]){
		
		String name = "Hello java";
		String name2 = new String("Hello java");
		System.out.println(name == name2);
		System.out.println(name.equals(name2));
		
		 }
	}
	```


> [!warning] Note
>  when you are using two string don't use ***==*** to check whether two string are equals.
>  Example : 

## References
- Webpage :
- Books   :
- Videos  :
