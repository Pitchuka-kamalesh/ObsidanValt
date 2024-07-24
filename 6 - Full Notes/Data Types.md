
2024-07-14 15:02

Status: #complete 

Tags:[[Java]]


---

# Data Types
---
##### notes:

> `Data Types` -> in java there are two Data Types *Primitive Datatype* and *nonprimitive Datatype*

> `Primitive Datatype` -> Primitive data are only single values and have no special capabilities.  There are 8 primitive data types. They are depicted below in tabular format below as follows:
> 

| Type    | Description             | Range of values                                            | implementation                                  |
| ------- | ----------------------- | ---------------------------------------------------------- | ----------------------------------------------- |
| boolean | true or false           | true,false                                                 | <p align="justify"></p>`boolean istrue = true;` |
| int     | twos-complement intger  | -2,147,483,648 to 2,147,483,647                            | `int number = 20;`                              |
| char    | Unicode character       | characters representation of ASCII values<br>0 to 255      | `char letter = 'a';`                            |
| byte    | twos-complement intger  | -128 to 127                                                | `byte value = 120;`                             |
| short   | twos-complement intger  | -32,768 to 32,767                                          | `short value = 30000;`                          |
| long    | twos-complement intger  | -9,223,372,036,854,775,808 to<br>9,223,372,036,854,775,807 | `long value = 3L;`                              |
| float   | IEEE 754 floating point | upto 7 decimal digits                                      | `float value = 3.14f;`                          |
| double  | IEEE 754 floating point | upto 16 decimal digits                                     | `double value = 5.1234568d;`                    |


> `Non - Primitive Datatype` -> The ****Reference Data Types**** will contain a memory address of variable values because the reference types won’t store the variable value directly in memory. They are strings, objects, arrays, etc.

| Type   | Description                                                                                                                                                                                                                                                                                                                                       | Notation                               |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
| Arrays | An _array_ is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed. You have seen an example of arrays already, in the `main` method of the "Hello World!" application. This section discusses arrays in greater detail. | `int[] anArray;anArray = new int[10];` |
| String | String is a sequences of Characters                                                                                                                                                                                                                                                                                                               | `String greeting = "Hello world!";`    |
-Array Notation
```java
Datatype[] names = {"Hello","Test","TestNG"};
```

> `Datatype[]` -> here we datatypes are primitive and nonprimitive datatypes are allowed

> `names` -> variable name  

> ` {"","",""};` -> values and these are located as a object reference with variable name we have access with variable name. 

```java
Datatype[] names = new Datatype[10];
for(int i = 0;i<name.length();i++){
	names[i] = "HEjj";

}
```

> `Datatype[] names = new Datatype[10];` -> here we are given the length to an array 

> `names[i] = "HEjj"` ->  here we are assigning value to its position.

> `index` -> Array index starts from 0 to 9;

```java
String varible_name = "sjwe=";
```

> `String ` -> String is non primitive data type 

> `"sjwe="` -> sequences of characters are Stored in memory location and address is assigned to varible_name
 
#### Reference Notes: 
 - ![[Pasted image 20240714152006.png]]
 - Two types of data types Primitive and nonprimitive data type 
 - primitive datatype are the build in the java building block the primitive datatype will store the variable value directly in memory.
 - ***types of primitive datatypes*** - *char* *boolean* *byte* *shot* *int* *long* *float* *double*
 - Non primitive datatype these are user defined data type and these stored the memory address of variable values because they won't store the variable value directly in memory.
 - ****types of nonprimitive datatypes**** - *String* *Arrays* *Class* *objects* *interfaces*

## References
- Webpage :[Java Data Types - GeeksforGeeks](https://www.geeksforgeeks.org/data-types-in-java/)
- Books   :
- Videos  :
