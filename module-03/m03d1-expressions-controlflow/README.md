# Module 03: Day 1 - Intro, Expressions & Control-Flow
Get into *real* programming, installing a development environment and then running our first programs and gaining knowledge of the basic building blocks of Java.

## Objectives
- Get a working environment going
- Create first program in Java
- Variables
- Expressions
- Control Flow
- Some of the Java *Lingo*

## Materials & Resources
### Environment
- download jdk (from Oracle, version 8) - this is the Java Development Kit; part of the challenge here is to figure out where to get this.  
- if *jre* (Java Runtime Environment) didn't download, get that too
- download the development environment tool: www.jetbrains.com - Install Intellij-IDEA; get the Ultimate edition (but ensure you get the license from a Mentor)


### Training
| Link | Comment| Time |
|:---- |:------ |-----:|
|https://www.youtube.com/watch?v=2Xa3Y4xz8_s|Historic background leading to Java (Guru-01)| 6:01|
|https://www.youtube.com/watch?v=qscQ3XT6qu4| Installing Java & IntelliJ IDEA (Koets)| 15:58|
|https://www.youtube.com/watch?v=TBWX97e1E9g |Getting started (Bana 01, note he's using eclipse)|17:42|
|https://www.youtube.com/watch?v=yYN8u90MKCg |Variables, Math functions & Scanner class (Bana 02)|17:05|
|https://www.youtube.com/watch?v=qZ2pb6BljLk |Conditional statement (Bana 03)|
|https://www.youtube.com/watch?v=efvZmFd1prA |Looping, collecting user input [with Scanner class] (Bana 04)|13:23|
|https://www.youtube.com/watch?v=r3DBIDyzLUI|Strings (mathtutordvd 07) - basic items|11:38|
|http://tutorials.jenkov.com/java/strings.html| resource on Java, specifically focused on strings||

### Optional
*If you've got time and/or want to dig deeper, consider the following:*

| Link | Comment| Time |
|:---- |:------ |-----:|
|https://www.youtube.com/watch?v=G1ubVOl9IBw|Understanding what the Java compiliation and run process (illustrated and compared to "c", (Guru-02)| 2:24|
|https://www.youtube.com/watch?v=yLkrw34VMNo |Clarifying JDK vs JRE and JVM, the components of Java (Prashun)||
|https://www.youtube.com/watch?v=L_jXj0XTwSg|Creating a new project using IntelliJ (IDEA)| 6:43|

|https://www.jetbrains.com/help/idea/2016.2/tutorial-creating-running-and-packaging-your-first-java-application.html |Using IDEA (instead of Eclipse)||
|https://www.youtube.com/watch?v=DnBTGtmJdzA|Alternative discussion on Variables and Binary (JCode.01)|5:19|
|https://www.youtube.com/watch?v=tUW2kIPY3is| Deeper on how memory works (storing variables. Stack & Heap) (JCode.02)|3:52|
|http://docs.oracle.com/javase/8/docs/api/java/lang/String.html|Official Java docs on Strings||

## Assignment Review
*Nothing from the previous session expected*


## Topics

### The Java environment
- Programs with the .java, .class extensions
- Compiling to bytecode
- RAM
- Just-in-time (JIT) compiling vs linking together
- Interpreter to machine code
- JDK, JRE, JVM

### "Hello World"
*Test that everything is installed correctly.*
- Get output
- Practice creating file, directories
- How to run a program
- `public static void main(string args[])`

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
 - char
 - String Class
 - length()
 - isEmpty()
 - Concatenation, concat()
 - Escape special characters
 - indexOf(), contains(), lastIndexOf()
 - substring()
 - format()
 - compareTo(), compareToIgnoreCase()
 - replace()
 - toLowerCase(), toUpperCase
 - trim()
 - \\, \n, \t
 *general familiarity with how to check syntax and find functions on the internet*

```java
// Strings and char                                                                                                                                           
// char 16 bit unicode character (unsigned -> min: 0; max: 65535)                                                                                             
String actionsProverb = "Actions speak louder than words.";                                                                                                   

// select the first char from the string, it is the uppercase A                                                                                               
char firstChar = actionsProverb.charAt(0);                                                                                                                    
System.out.println(firstChar);                                                                                                                                

// string concatenation                                                                                                                                       
String concated = "Hope for the best " + "but";                                                                                                               
concated = concated + " prepare";                                                                                                                             
concated += " for ";                                                                                                                                          
concated.concat("the worst.");                                                                                                                                
System.out.println(concated);                                                                                                                                 

// escape special character                                                                                                                                   
String strWithSpecialCharacters = "I can \"put\" special 'characters' in a \\string\\.";                                                                      
System.out.println(strWithSpecialCharacters);                                                                                                                 

// length of a string                                                                                                                                         
int myLength = "what is my length?".length();                                                                                                                 
System.out.println(myLength);                                                                                                                                 

System.out.println(actionsProverb.length());                                                                                                                  

// isEmpty()                                                                                                                                                  
String emptyString = "";                                                                                                                                      
System.out.println("Is \"emptyString\" empty? " + emptyString.isEmpty());                                                                                     
System.out.println("Is \"actionsProverb\" empty? " + actionsProverb.isEmpty());                                                                               

// contains                                                                                                                                                   
System.out.println(actionsProverb.contains("than")); // true                                                                                                  
System.out.println(actionsProverb.contains("five")); // false                                                                                                 

// indexOf                                                                                                                                                    
System.out.println(actionsProverb.indexOf("t")); // 2 (t in "Actions")                                                                                        
System.out.println(actionsProverb.indexOf("t", 3)); // second parameter is called fromIndex, result will be 21 (t in "than")                                  
System.out.println(actionsProverb.indexOf("thinking")); // -1                                                                                                 

// lastIndexOf                                                                                                                                                
System.out.println(actionsProverb.lastIndexOf("t")); // 21 (t in "than")                                                                                      

// substring                                                                                                                                                  
System.out.println(actionsProverb.substring(0,7)); // result will be "Actions"                                                                                
System.out.println(actionsProverb.substring(14,20)); // result will be "louder" (startIndex, endIndex)                                                        

// format strings                                                                                                                                             
System.out.println(String.format("I have %d cats.", 2)); // %d -> integer                                                                                     
System.out.println(String.format("I have %d %s and I love them!", 3, "raptors")); // %d -> integer; %s -> string, %f -> float                                 

// compareTo                                                                                                                                                  
System.out.println("a".compareTo("b")); // -1                                                                                                                 
System.out.println("b".compareTo("a")); // 1                                                                                                                  
System.out.println("a".compareTo("c")); // -2                                                                                                                 
System.out.println("a".compareTo("deli")); // -3                                                                                                              
System.out.println("a".compareTo("a")); // 0 -> equals                                                                                                        

// compareToIgnoreCase                                                                                                                                        
System.out.println("a".compareToIgnoreCase("A")); // 0 -> equals                                                                                              

// replace                                                                                                                                                    
String weakestLinkProverb = "A rope is only as strong as its weakest link."; // it has a mistake, correctly: "A chain is only as strong as its weakest link."
System.out.println(weakestLinkProverb.replace("rope", "chain"));                                                                                              
System.out.println(weakestLinkProverb.replace("a", "b"));                                                                                                     

// toLowerCase; toUpperCase                                                                                                                                   
System.out.println("How much is the fish?".toUpperCase());                                                                                                    
System.out.println("HOOOORRRAAAAAYYYY".toLowerCase());                                                                                                        

// trim                                                                                                                                                       
System.out.println("     string with lots of spaces       ".trim());                                                                                          
```

#### Other datatypes
- Boolean
```java
// Boolean (8 bit, 1 byte), true or false         
Boolean trueCondition = Boolean.TRUE;             
System.out.println(trueCondition); // true        
```
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

```java
// Conditionals                                                                                 
// Example 1                                                                                    
if(1 == 1)                                                                                      
    System.out.println("1 equals 1, wohooo");                                                   

// Example 2                                                                                    
if(2 >= 1)                                                                                      
    System.out.println("2 is greater than or equal to 1");                                      

// Example 3 (!= not equal)                                                                     
if(4 != 5)                                                                                      
    System.out.println("4 is not equal to 5");                                                  

// Example 4                                                                                    
int a = 5;                                                                                      
int b = 7;                                                                                      

if(a > b) {                                                                                     
    System.out.println(String.format("%d is bigger than %d", a, b));                            
} else {                                                                                        
    System.out.println(String.format("%d is less than %d", a, b));                              
}                                                                                               
// What happens when a equals b? (Let's see Example 3)                                          

// Example 5                                                                                    
b = 5;                                                                                          

if(a > b) {                                                                                     
    System.out.println(String.format("%d is bigger than %d", a, b));                            
} else if(a < b) {                                                                              
    System.out.println(String.format("%d is less than %d", a, b));                              
}else {                                                                                         
    System.out.println(String.format("%d is equals to %d", a, b));                              
}                                                                                               

// Example 6 -> check if "a" is in the 1..9 range (inclusive)                                   
a = 5;                                                                                          

if(a >= 1 && a <=9) {                                                                           
    System.out.println("It is in the range!");                                                  
}                                                                                               

// Example 7 -> check if "a" is outside of the 1..9 range (use conditional "or" operator)       
a = -2;                                                                                         

if(a < 1 || a > 9)                                                                              
    System.out.println("\"a\" is outside of the specified range.");                             

// Example 8 -> check if "a" is outside of the 1..9 range, but with using negation operator (!)
a = -2;                                                                                         

if(!(a >= 1 && a <=9)) {                                                                        
    System.out.println("\"a\" is outside of the specified range.");                             
}                                                                                               

// Example 9                                                                                    
Boolean trueBool = true;                                                                        
Boolean falseBool = Boolean.FALSE;                                                              

if(trueBool || falseBool)                                                                       
    System.out.println("One of the variables is \"true\"");                                     
```

- bitwise operators
   - and &
   - or |
   - xor ^

### Loops
- for
- while
- do while
- break
- continue

```java
// Loops                                                                        
// For statement/loop                                                           
/*                                                                              
    for (initialization; termination; increment) {                              
        statement(s)                                                            
    }                                                                           
*/                                                                              

// Example 1                                                                    
for (int i = 0; i < 10; i++) {                                                  
    System.out.print(i);                                                        
}                                                                               

// Example 2 -> going by 2                                                      
int j = 0;                                                                      
for (; j < 10; j += 2)                                                          
    System.out.print(j);                                                        

// Example 3 -> infinity loop ( :D )                                            
for(;;)                                                                         
    System.out.print(j);                                                        

// While statement/loop                                                         
/*                                                                              
    while (expression) {                                                        
        statement(s)                                                            
    }                                                                           
*/                                                                              

// Example 1                                                                    
int k = 0;                                                                      
while (k < 10) {                                                                
    System.out.print(k);                                                        
    k++;                                                                        
}                                                                               

// Example 2                                                                    
k = 0;                                                                          
while (k < 10) {                                                                
    System.out.print(k);                                                        
    k += 2;                                                                     
}                                                                               

// Do-While statement/loop (it executes at least once)                          
/*                                                                              
    while (expression) {                                                        
        statement(s)                                                            
    }                                                                           
*/                                                                              

// Example 1                                                                    
int l = 0;                                                                      
do {                                                                            
    System.out.print(l);                                                        
    l++;                                                                        
} while (l < 10);                                                               

// Example 2                                                                    
l = 0;                                                                          
do {                                                                            
    System.out.print(l);                                                        
    l += 2;                                                                     
} while (l < 10);                                                               


// Break statement (jump out from the loop)                                     

// Example 1 -> break when  the first element has found which is divisible by 5
for (int m = 1; m < 10; m++) {                                                  
    if (m % 5 == 0)                                                             
        break;                                                                  
    System.out.print(m);                                                        
}                                                                               


// Continue statement (jump to the next loop iteration)                         

// Example 1 -> continue on elements which is divisible by 2                    
for (int m = 1; m < 10; m++) {                                                  
    if (m % 2 == 0)                                                             
        continue;                                                               
    System.out.print(m);                                                        
}                                                                               
```


## Workshop/Practice

### Challenge 
### Challenge 
- https://www.codewars.com/kata/563f037412e5ada593000114/train/java - Interest rate computation


## Assignment
- Loop printing out prime numbers from 2 to 100

# Links
- [Return to Module Overview](..)
- Previous day - (not applicable)
- [Next day](../m03d2-arrays-collections-functions)