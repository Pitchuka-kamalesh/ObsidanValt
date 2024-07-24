---
date: 2024-07-15
Topic: Operators
Subtopics: binary and Arithmetical Operators
tags:
  - "#adult"
Links:
  - "[[Java]]"
Task: 
cssclasses:
  - wide-page
---
~~~tabs
tab: increment/Decrement operators
|operant|description|
|----|----|
|`i++`|post increment operator|
|`++i`|pre increment operator|
|`i--`|post decrement operator|
|`--i`|pre decrement operator|
tab: Arithmetic operators
|operant|description|
|----|----|
| `-` | it is used to substract to numarical value |
|`+`| it is used to add the numarical and String values |
|`*`| it is used to muliplication of two numarical values |
|`/`| it will divide the numarical and will give quotient|
|`%`| it will divide the numarical values and will give remainder |
~~~
~~~tabs
tab: Relational and boolean Operators
|  operant   | Description  |
| --- | --- |
|==| Equals operator is used to check both the values having same then it will return boolean value|
|!=| notEquals operator is used to check both the values not having same then it will return boolean value |
| < | less than operant is used the check the given value is less that the second value it will return boolean value |
| <= | lessthan Equalto operant is used the check the given value is lessthan and equalto that the second value it will return boolean value  |
| > | greater than operant is used the check the given value is more that the second value it will return boolean value |
| >= | greater than Equalto operant is used the check the given value is greater and equalto that the second value it will return boolean value |
| && | logical and operant is used to check two conditions if both are true then it retur true otherwise false |
tab: Bitwise Operators
|  operant   | Description  |
| --- | --- |
|     |     |
~~~


---

#### Operators Code 
---
## increment/Decrement operators
~~~tabs
tab: post increment

```java
class HelloWorld {
    public static void main(String[] args) {
        int i = 10;
        System.out.println("i value before increment -> "+ i);
        System.out.println("i value using i++ post increment operator -> "+(i++));
        System.out.println("i value after post increment i++ -> " + i);
    }
}
```
> output 
>> i value before increment -> 10
>> i value using `i++` post increment operator -> 10
>> i value after post increment `i++` -> 11

tab: pre increment

```java
class HelloWorld {
    public static void main(String[] args) {
	    int i = 10;  
		System.out.println("i value before increment -> "+ i);  
		System.out.println("i value using ++i pre increment operator -> "+(++i));  
		System.out.println("i value after pre increment ++i -> " + i);
    }
}

```
> output
>> i value before increment -> 10
>> i value using `++i` pre increment operator -> 11
>> i value after pre increment `++i` -> 11

tab: post decrement

```java
public class Testers {  
    public static void main(String[] args) {  
        int i = 10;  
        System.out.println("i value  -> "+ i);  
        System.out.println("i value using i-- post decrement operator -> "+(i--));  
        System.out.println("i value after post decrement operator i-- -> " + i);  
  
  
    }  
}

```
> output 
>> i value  -> 10
>> i value using `i--` post decrement operator -> 10
>> i value after post decrement operator `i--` -> 9

tab: pre decrement

```java
public class Testers {  
    public static void main(String[] args) {  
        int i = 10;  
        System.out.println("i value  -> "+ i);  
        System.out.println("i value using --i pre decrement operator -> "+(--i));  
        System.out.println("i value after pre decrement operator --i -> " + i);  
  
    }  
}

```
> output 
>> i value  -> 10
>> i value using `--i` pre decrement operator -> 9
>> i value after pre decrement operator `--i` -> 9
~~~
---

## Arithmetical operation 
 
~~~tabs
tab: Add +
```java
class HelloWorld {
    public static void main(String[] args) {
        int i = 10;
        int j = 20;
        System.out.println("sum + of two numbers -> "+ (i+j));
    }
}

``` 
> output :
>> sum `+` of two numbers -> 30

tab: Sub -
```java
class HelloWorld {
    public static void main(String[] args) {
        int i = 10;
        int j = 20;
        System.out.println("difference -  of two numbers -> " + (i-j));
    }
}

```
> output :
>> difference `-` of two numbers -> -10

tab: multiplication *
```java
class HelloWorld {
    public static void main(String[] args) {
        int i = 10;
        int j = 20;
        System.out.println("Multiplication * of two numbers -> "+(i*j));
    }
}

```
> output: 
>>  Multiplication `*` of two numbers -> 200

tab: division /
```java
public class Testers {  
    public static void main(String[] args) {  
        int i = 10;  
        int j = 26;  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        System.out.println("division / of integer numbers -> "+ (j/i));  
        System.out.println("division  / of float numbers -> "+ (f2/f1));  
    }  
}
```
> output: 
>> division `/` of integer numbers -> 2
>> division  `/` of float numbers -> 2.6

tab: modules %
```java
public class Testers {  
    public static void main(String[] args) {  
        int i = 10;  
        int j = 26;  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        System.out.println("modules of integer numbers -> "+ (j%i));  
        System.out.println("modules of float numbers -> "+ (f2%f1));  
  
    }  
}
```
> output:
>> modules `%` of integer numbers -> 6
>> modules `%` of float numbers -> 6.0
~~~

---

## Relational and boolean Operators


~~~tabs
tab: ==
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `==` in two integer variable -> "+ i + " == " +j+ "-> "+ (i==j));  
        System.out.println("using `==` in two integer variable -> "+ i + " == " +k+ "-> "+ (i==k));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `==` in two float variable -> "+ f1 + " == " +f2+ "-> "+ (f1==f2));  
        System.out.println("using `==` in two float variable -> "+ f1 + " == " +f3+ "-> "+(f1==f3));  
  
//      String Variables  
        String name1 = "HelloWorld";  
        String name2 = "HelloWorld";  
        String name3 = new String("HelloWorld");  
        System.out.println("using `==` in two  Strings -> "+ name1 + " == " +name2+ "-> "+ (name1==name2));  
        System.out.println("using `==` in two  String -> "+ name1 + " == " +name3+ "-> "+(name1==name3));  
  
  
  
    }  
}

``` 
> output
>> using ***==*** in two integer variable -> 10 == 26-> false
>> using ***==*** in two integer variable -> 10 == 10-> true
>> using ***==*** in two float variable -> 10.0 == 26.0-> false
>> using ***==*** in two float variable -> 10.0 == 10.0-> true
>> using ***==*** in two  Strings -> HelloWorld == HelloWorld-> true
>>using ***==*** in two  String -> HelloWorld == HelloWorld->false


tab: !=
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `!=` in two integer variable -> "+ i + " != " +j+ "-> "+ (i!=j));  
        System.out.println("using `!=` in two integer variable -> "+ i + " != " +k+ "-> "+ (i!=k));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `!=` in two float variable -> "+ f1 + " != " +f2+ "-> "+ (f1!=f2));  
        System.out.println("using `!=` in two float variable -> "+ f1 + " != " +f3+ "-> "+(f1!=f3));  
  
//      String Variables  
        String name1 = "HelloWorld";  
        String name2 = "HelloWorld";  
        String name3 = new String("HelloWorld");  
        System.out.println("using `!=` in two  Strings -> "+ name1 + " != " +name2+ "-> "+ (name1!=name2));  
        System.out.println("using `!=` in two  String -> "+ name1 + " != " +name3+ "-> "+(name1!=name3));  
  
  
  
    }  
}

``` 
> output
>> using `!=` in two integer variable -> 10 != 26 -> true
>> using `!=` in two integer variable -> 10 != 10 -> false
>> using `!=` in two float variable -> 10.0 != 26.0 -> true
>> using `!=` in two float variable -> 10.0 != 10.0 -> false
>> using `!=` in two  Strings -> HelloWorld != HelloWorld -> false
>> using `!=` in two  String -> HelloWorld != HelloWorld -> true

tab: <
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `<` in two integer variable -> "+ i + " < " +j+ "-> "+ (i<j));  
        System.out.println("using `<` in two integer variable -> "+ i + " < " +k+ "-> "+ (i<k));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `<` in two float variable -> "+ f1 + " < " +f2+ "-> "+ (f1<f2));  
        System.out.println("using `<` in two float variable -> "+ f1 + " < " +f3+ "-> "+(f1<f3));  
          
    }  
}

``` 
> output
>> using `<` in two integer variable -> 10 < 26-> true
>> using `<` in two integer variable -> 10 < 10-> false
>> using `<` in two float variable -> 10.0 < 26.0-> true
>> using `<` in two float variable -> 10.0 < 10.0-> false 

tab: <=
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `<=` in two integer variable -> "+ i + " <= " +j+ "-> "+ (i<=j));  
        System.out.println("using `<=` in two integer variable -> "+ i + " <= " +k+ "-> "+ (i<=k));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `<=` in two float variable -> "+ f1 + " <= " +f2+ "-> "+ (f1<=f2));  
        System.out.println("using `<=` in two float variable -> "+ f1 + " <= " +f3+ "-> "+(f1<=f3));  
  
    }  
}

``` 
> output
>> using `<=` in two integer variable -> 10 <= 26 -> true
>> using `<=` in two integer variable -> 10 <= 10 -> true
>> using `<=` in two float variable -> 10.0 <= 26.0 -> true
>> using `<=` in two float variable -> 10.0 <= 10.0 -> true
tab: >
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `>` in two integer variable -> "+ i + " > " +j+ " -> "+ (i>j));  
        System.out.println("using `>` in two integer variable -> "+ i + " > " +k+ " -> "+ (i>k));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `>` in two float variable -> "+ f1 + " > " +f2+ " -> "+ (f1>f2));  
        System.out.println("using `>` in two float variable -> "+ f1 + " > " +f3+ " -> "+(f1>f3));  
  
    }  
}

``` 
> output
>> using `>` in two integer variable -> 10 > 26 -> false
>> using `>` in two integer variable -> 10 > 10 -> false
>> using `>` in two float variable -> 10.0 > 26.0 -> false
>> using `>` in two float variable -> 10.0 > 10.0 -> false
tab: >=
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `>=` in two integer variable ->= "+ i + " >= " +j+ " ->= "+ (i>=j));  
        System.out.println("using `>=` in two integer variable ->= "+ i + " >= " +k+ " ->= "+ (i>=k));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `>=` in two float variable ->= "+ f1 + " >= " +f2+ " ->= "+ (f1>=f2));  
        System.out.println("using `>=` in two float variable ->= "+ f1 + " >= " +f3+ " ->= "+(f1>=f3));  
  
    }  
}

``` 
> output
>> using `>=` in two integer variable ->= 10 >= 26 ->= false
>> using `>=` in two integer variable ->= 10 >= 10 ->= true
>> using `>=` in two float variable ->= 10.0 >= 26.0 ->= false
>> using `>=` in two float variable ->= 10.0 >= 10.0 ->= true

tab: &&
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `&&` in two integer variable -> "+ (i==j) + " && " +(j!=k)+ " -> "+ ((i==j)&&(j!=k)));  
        System.out.println("using `&&` in two integer variable ->  "+ (i==j) + " && " +(j==k)+ " ->  "+  ((i==j)&&(j==k)));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `&&` in two float variable -> "+ (f1==f2) + " && " + (f1!=f3)+ " -> "+  ((f1==f2)&&(f1!=f3)));  
        System.out.println("using `&&` in two float variable -> "+ (f1==f2)+ " && " +(f1==f3)+ " -> "+((f1==f2)&&(f1==f3)));  
  
    }  
}

``` 
> output
>> using `&&` in two integer variable -> false && true -> false
>> using `&&` in two integer variable ->  false && false ->  false
>> using `&&` in two float variable -> false && false -> false
>> using `&&` in two float variable -> false && true -> false>> 

tab: ||
```java
public class Testers {  
    public static void main(String[] args) {  
//      Integer Variables  
        int i = 10;  
        int k = 10;  
        int j = 26;  
  
        System.out.println("using `||` in two integer variable -> "+ (i==j) + " || " +(j!=k)+ " -> "+ ((i==j)||(j!=k)));  
        System.out.println("using `||` in two integer variable ->  "+ (i==j) + " || " +(j==k)+ " ->  "+  ((i==j)||(j==k)));  
  
  
//      Float Variables  
        float f1 = 10.00f;  
        float f2 = 26.00f;  
        float f3 = 10.00f;  
        System.out.println("using `||` in two float variable -> "+ (f1==f2) + " || " + (f1!=f3)+ " -> "+  ((f1==f2)||(f1!=f3)));  
        System.out.println("using `||` in two float variable -> "+ (f1==f2)+ " || " +(f1==f3)+ " -> "+((f1==f2)||(f1==f3)));  
  
    }  
}

``` 
> output
>> using `||` in two integer variable -> false || true -> true
>> using `||` in two integer variable ->  false || false ->  false
>> using `||` in two float variable -> false || false -> false
>> using `||` in two float variable -> false || true -> true
~~~
---



## References
- Webpage :
- <span style="background:#9254de">Operators</span> : [[Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013.pdf#page=71&selection=0,5,0,14|Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013, page 71]]
- <span style="background:#9254de">Increment and Decrement Operators</span> : [[Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013.pdf#page=72&selection=35,6,35,40|Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013, page 72]]
- <span style="background:#9254de">Relational and boolean Operators</span> : [[Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013.pdf#page=72&selection=167,6,171,9|Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013, page 72]]
- <span style="background:#9254de">Bitwise Operators</span> : [[Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013.pdf#page=73&selection=171,6,171,24|Core Java Volume I- Fundamentals 9th Edition- Horstmann, Cay S. & Cornell, Gary_2013, page 73]]
- Code: