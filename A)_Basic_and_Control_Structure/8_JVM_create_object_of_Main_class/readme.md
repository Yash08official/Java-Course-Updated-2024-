### Does JVM create object of Main class (the class with main())?

Consider following program.<br>

```
class Main {
    public static void main(String args[])
    {
        System.out.println("Hello");
    }
}
```

<br>
<b>Output :</b>
<em>Hello</em>
<br>

Does JVM create an object of class Main?
The answer is "No". We have studied that the reason for main() static in Java is to make sure that the main() can be called without any instance. To justify the same, we can see that the following program compiles and runs fine.

```
// Note Main is abstract
abstract class Main {
    public static void main(String args[])
    {
        System.out.println("Hello");
    }
}

```

<br>

<b>Output :</b>
<em>Hello</em>
<br>

Since we can't create object of abstract classes in Java, it is guaranteed that object of class with main() is not created by JVM.
