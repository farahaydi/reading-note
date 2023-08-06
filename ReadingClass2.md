**Use an analogy to explain Built-In packages. Give examples.**
Built-in packages are existing java packages that come along with the JDK. 
For example, 
- java.lang
- java.util
- java.io

For example:
import java.util.ArrayList;

class ArrayListUtilization {
    public static void main(String[] args) {

        ArrayList<Integer> myList = new ArrayList<>(3);
        myList.add(3);
        myList.add(2);
        myList.add(1);

        System.out.println(myList);
    }}


**How to create a package in Intellij IDEA?**
In IntelliJ IDEA, here's how you can create a package:

- Right-click on the source folder.
- Go to new and then package.
- A pop-up box will appear where you can enter the package name.

**Which loop types use a loop counter?**
For Loop

**Explain the difference between While and Do-While loops.**
>While Loop:
In a "while" loop, the loop condition is evaluated before executing the loop body. If the condition is true, the loop body is executed, and then the condition is checked again. If the condition is still true, the loop body continues to execute, and this process repeats until the condition becomes false. If the condition is false initially, the loop body will not be executed at all.
>Do-While Loop:
In a "do-while" loop, the loop body is executed at least once before checking the loop condition. Once the loop body is executed, the condition is evaluated. If the condition is true, the loop body will be executed again, and the process repeats until the condition becomes false.

**Describe 3 built-in methods for Arrays.**
- append()
- pop()
- index()

**How is the size of an array determined in Java?**
dataType[] arrayName = new dataType[arraySize];



