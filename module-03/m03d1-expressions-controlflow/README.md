# Module 03: Day 1 - Intro, Expressions & Control-Flow
*Describe the days objectives*

## Materials & Resources
### INTRO/SET ENV
- download jdk (from Oracle, version 8)
- if jre didn't download, get that too
- download the development environment tool: www.jetbrains.com - Install Intellij-IDEA


### JAVA
| Link | Comment |
|:---- |:------- |
| https://www.youtube.com/watch?v=2Xa3Y4xz8_s | What is Java|
| https://www.youtube.com/watch?v=yLkrw34VMNo |The components of Java |
| https://www.jetbrains.com/help/idea/2016.2/tutorial-creating-running-and-packaging-your-first-java-application.html ||
| https://www.youtube.com/watch?v=TBWX97e1E9g | Bana video on getting started (using eclipse)|
| https://www.youtube.com/watch?v=yYN8u90MKCg | Bana variables |
| https://www.youtube.com/watch?v=qZ2pb6BljLk ||
| https://www.youtube.com/watch?v=efvZmFd1prA ||
| https://www.youtube.com/watch?v=TBWX97e1E9g ||
| https://www.youtube.com/watch?v=RxeDe6BsTMI|String functions|


### Optional
*If you've got time, consider the following:*
| Link | Comment |
|:---- |:------- |
|https://www.youtube.com/watch?v=G1ubVOl9IBw||
|https://www.youtube.com/watch?v=DnBTGtmJdzA| Variables and Binary|
|https://www.youtube.com/watch?v=tUW2kIPY3is| What is memory|


## Assignment Review
*Nothing from the previous session expected*

## Topics

### The Java environment
- Programs with the .java extension
- Compiling to bytecode
- Linked together
- Interpreter

### "Hello World"
*Test that everything is installed correctly*
- Get output
- Practice creating file, directories
- How to run a program

```java
System.out.println("Hello world!");
```

### Variables
#### Numbers
- Integer
- Byte
- Short
- Long
- Float
- Double
- Range limitations
- Arithmetic Operators (+, -, *, /, %, ++, --, +=, -=, /=, *=)

```java
      // Integers
      // Byte (8 bit; min:-128; max: +127)
      byte a = -127;
      byte b = 2;
      byte c = 278; // error by the IDE

      // Short (16 bit; min: -32768 ; max: +32 767)
      short d = -32768;
      short e = 65000; // error by the IDE
      Short f = 567;

      // Integer (32 bit; min: -2 147 483 648; max: 2 147 483 647)
      int g = 12;
      Integer h = 13;


      // Long (64 bit; min: -9 223 372 036 854 775 808 ;max: 9 223 372 036 854 775 807 )
      long i = 200;
      long j = 30000000000000L;
      long k = -34500000000L;

      // Floats
      // Float (32 bit single precision IEEE 754)
      float l = 1.3f;
      float m = 45f;
      Float n = 0; // use 0f

      // Double ( 64 bit, double precision IEEE 754)
      double o = 23.03013103103d;
      Double p = 1d;

      // Arithmetic operators
      int aa = 3 + 4;
      int bb = 6 * 7;
      int cc = 8 / 4;
      int dd = 8 % 4;
      int ee = 8 % 5;

      int ff = 8;
      ff *= 3;
      ff /= 6; // ff = 4
```


#### Strings
http://docs.oracle.com/javase/8/docs/api/java/lang/String.html
 - char
 - String Class
 - length
 - isEmpty()
 - Concatenation
 - indexOf(), contains()
 - substring()
 - format()
 - compareTo
 - replace
 - toLowerCase(), toUpperCase
 - trim()
 *general familiarity with how to check syntax and find functions on the internet*

#### Other datatypes
- Boolean
- Date (will cover later)
- Objects (will cover later)

### Conditional
- comparison operators
  - ==      equal to
  - !=      not equal to
  - >       greater than
  - >=      greater than or equal to
  - <       less than
  - <=      less than or equal to
- if
- else
- elseif
- switch
- conditional operators
   - and &&
   - or ||
   - negation !
   - xor ^

- bitwise operators
   - and &
   - or |
   - negation !

### Loops
- for
- while
- do while
- break
- continue


## Workshop/Practice

### Challenge 1
### Challenge Final
- https://www.codewars.com/kata/563f037412e5ada593000114/train/java - Interest rate computation


## Assignment
