# Enum with Customized Value in Java

Prerequisite : enum in Java

By default enums have their own string values, we can also assign some custom values to enums. Consider below example for that.

Examples:

```
{
    APPLE(“RED”), BANANA(“YELLOW”), GRAPES(“GREEN”);
}
```

In above example we can see that the Fruits enum have three members i.e APPLE, BANANA and GRAPES with have their own different custom values RED, YELLOW and GREEN respectively.

##### Now to use this enum in code, there are some points we have to follow:-

We have to create parameterized constructor for this enum class. Why? Because as we know that enum class’s object can’t be create explicitly so for initializing we use parameterized constructor. And the constructor cannot be the public or protected it must have private or default modifiers. Why? if we create public or protected, it will allow initializing more than one objects. This is totally against enum concept.

#### 1. We have to create one getter method to get the value of enums.

## Java

```java
// Java program to demonstrate how values can
// be assigned to enums.
enum TrafficSignal
{
    // This will call enum constructor with one
    // String argument
    RED("STOP"), GREEN("GO"), ORANGE("SLOW DOWN");

    // declaring private variable for getting values
    private String action;

    // getter method
    public String getAction()
    {
        return this.action;
    }

    // enum constructor - cannot be public or protected
    private TrafficSignal(String action)
    {
        this.action = action;
    }
}

// Driver code
public class EnumConstructorExample
{
    public static void main(String args[])
    {
        // let's print name of each enum and there action
        // - Enum values() examples
        TrafficSignal[] signals = TrafficSignal.values();

        for (TrafficSignal signal : signals)
        {
            // use getter method to get the value
            System.out.println("name : " + signal.name() +
                        " action: " + signal.getAction() );
        }
    }
}
```
Output:
name : RED action: STOP
name : GREEN action: GO 
name : ORANGE action: SLOW DOWN 