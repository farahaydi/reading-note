**1-Explain the difference between an “int” and an “Integer” in Java.**
>int:
"int" is a primitive data type in Java. It represents a 32-bit signed integer value. As a primitive type, it's not an object and doesn't have any methods or additional properties associated with it. It's very efficient in terms of memory and performance since it directly stores the value in memory without any overhead.
Integer:
"Integer" is a class in Java that belongs to the java.lang package. It's a wrapper class that provides an object representation of the primitive int data type. It allows you to treat an int as an object and provides various methods for performing operations on integers. 

//===============================================================//

**2-What is the default value for ints? Integers?**
>int:
The default value for an "int" primitive data type in Java is 0. 
Integer:
The default value for an "Integer" object (a reference type) is null.

//==============================================================//

**3-What is autoboxing? Unboxing?**

>Both are convenient for switching between primitive types and objects, but excessive use can impact performance.
Autoboxing: Autoboxing involves the automatic conversion between primitive data types and their corresponding wrapper classes.
int primitiveInt = 42;
Integer wrapperInt = primitiveInt; ==> primitiveInt will be obj from Integer class
Unboxing: Automatic conversion of wrapper class objects back to primitive types.
Integer wrapperInt = 42;
int primitiveInt = wrapperInt;  ==>wrapperInt will be primetive data type.

//=============================================================//

**4-List the three basic categories of exceptions.**
>-IndexOutOfBoundsException 
>-Checked Exceptions
>-NullPointerException

//============================================================//
**5-What type of statement can you use to handle an exception?**

The try-catch statement.

//===========================================================//
**6-Describe a situation where you think it would be useful to have a program that scans text.**

>The Scanner class is used to break down input into tokens based on white space (blanks, tabs, line terminators) by default.
The example program ScanXan reads words from a file and prints them one per line.
To change the token separator, you can use useDelimiter() with a regular expression.
Scanner supports various data types and can translate tokens accordingly, including numeric values with locale-specific formatting.
The ScanSum example reads double values from a file, adds them up, and uses the US locale for proper numeric interpretation.
The Scanner object should be closed after use to indicate that the underlying resources are done being used.

//==========================================================//

**7-What is input from a Scanner broken down into?**

>Input from a Scanner is broken down into tokens. 

