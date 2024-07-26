### Naming Conventions in Java

A programmer is always said to write clean codes, where naming has to be appropriate so that for any other programmer it acts as an easy way out to read the code. At a smaller level, this seems meaningless but think of the industrial level where it becomes necessary to write clean codes in order to save time for which there are certain rules been laid of which one of the factors is to name the keyword right which is termed as a naming convention in Java.

For example when you are using a variable name depicting displacement then it should be named as "displace" or similar likewise not likely x, d which becomes complex as the code widens up and decreases the readability aperture. Consider the below illustrations to get a better understanding which later on we will be discussing in detail.

<h3>Illustrations: </h3>
<ul>
<li>Class</li>
If you are naming any class then it should be a noun and so should be named as per the goal to be achieved in the program such as Add2Numbers, ReverseString, and so on not likely A1, Programming, etc. It should be specific pointing what exactly is there inside without glancing at the body of the class.
<li>Interface</li>
If you are naming an interface, it should look like an adjective such as consider the existing ones: Runnable, Serializable, etc. Try to use 'able' at the end, yes it is said to try as there are no hard and fast bound rules as if we do consider an inbuilt interface such as 'Remote', it is not having ble at the end. Consider if you are supposed to create an interface to make read operation then it is suggested as per naming conventions in java to name a similar likely 'Readable' interface.
<li>Methods</li>
Now if we do look closer a method is supposed to do something that it does contains in its body henceforth it should be a verb.
<li>Constants</li>
As the name suggests it should look like as we read it looks like it is fixed for examples PI, MAX_INT, MIN_INT, etc. as follows.
</ul>

<h2>Naming Conventions in Java  </h2>
In java, it is good practice to name class, variables, and methods name as what they are actually supposed to do instead of naming them randomly. Below are some naming conventions of the java programming language. They must be followed while developing software in java for good maintenance and readability of code. Java uses CamelCase as a practice for writing names of methods, variables, classes, packages, and constants. 
<br>
Camel's case in java programming consists of compound words or phrases such that each word or abbreviation begins with a capital letter or first word with a lowercase letter, rest all with capital. Here in simpler terms, it means if there are two 
<br>
Note: Do look out for these exception cases to camel casing in java as follows:

<ul>
<li>In package, everything is small even while we are combining two or more words in java</li>
<li>In constants, we do use everything as uppercase and only '_' character is used even if we are combining two or more words in java.</li>
</ul>

<h2>Type 1: Classes and Interfaces</h2>
<ul>
<li>Class names should be nouns, in mixed cases with the first letter of each internal word capitalized. Interfaces names should also be capitalized just like class names.</li>
<li>Use whole words and must avoid acronyms and abbreviations.</li>

```
Classes: class Student { }
         class S=Integer {}
         class Scanner {}
```

```
Interfaces : Runnable
             Remote
             Serializable
```

<h2>Type 2: Methods </h2>
<li>Methods should be verbs, in mixed case with the first letter lowercase and with the first letter of each internal word capitalized.</li>

```
public static void main(String [] args)  {}

```

As the name suggests the method is supposed to be primarily method which indeed it is as main() method in java is the method from where the program begins its execution.

<h2>Type 3: Variables</h2>

Variable names should be short yet meaningful.

Variable names should not start with underscore \_ or dollar sign $ characters, even though both are allowed.

<ul>
<li>Should be mnemonic i.e., designed to indicate to the casual observer the intent of its use.</li>
<li>One-character variable names should be avoided except for temporary variables</li>
<li>Common names for temporary variables are i, j, k, m, and n for integers; c, d, and e for characters.</li> 
</ul>
</ul>

```
int[] marks;
double double answer,
```

As the name suggests one stands for marks while the other for an answer be it of any e do not mind.

<h2>Type 4: Constant variables</h2>
<ul>
<li>Should be all uppercase with words separated by underscores ("_").</li>
<li>There are various constants used in predefined classes like Float, Long, String etc.</li>
```
num = PI;
```
</ul>

<h2>Type 5: Packages</h2>
<ul>
<li>The prefix of a unique package name is always written in all-lowercase ASCII letters and should be one of the top-level domain names, like com, edu, gov, mil, net, org.</li>
<li>Subsequent components of the package name vary according to an organization's own internal naming conventions.</li>
</ul>

```
java.util.Scanner ;
java.io.*;
```

As the name suggests in the first case we are trying to access the Scanner class from the java.util package and in other all classes(* standing for all) input-output classes making it so easy for another programmer to identify.

Note:

For class and interfaces, the first letter has to be uppercase.
For method , variable, package_name, and constants, the first letter has to be lowercase.