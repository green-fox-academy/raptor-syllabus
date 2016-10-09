# Module 03: Day 2 - Array, Functions and Debugging & Exceptions
Expanding for the the primitive datatypes, computers also work with lists of data; one of the most basic is the *arrays*.  Arrays offer a way to process a list of items, applying the same rules; and collecting a series of results for reporting.
Additionally, as we are now conversant with the basic data types and flow, we introduce some tools so that we can watch what is happening when a program runs, find where a program does the __bad__ thing (that is to say, *goes awry*) and instruct it on how to handle exceptions.
Also, we show how we can extend the environment with features developed by others (i.e. libraries).


## Materials & Resources
- One of the examples makes use of a library that is available over the internet (from a source called Maven).  Called `commons-lang` you will need it for use in the Array exercise.

| Link | Comment|
|:---- |:------ |
|https://www.youtube.com/watch?v=1HTsLK_m2ao|Methods & Fields, Using Functions (Bana 05)|
|https://www.youtube.com/watch?v=eNPX2pTiaHI|Bana 09 (before 08!)|
|https://www.youtube.com/watch?v=EWj60p8esD0|Exceptions: Try/Catch|
|https://www.youtube.com/watch?v=rGlJiUO-dZA|Functions with Classes |
|https://www.youtube.com/watch?v=_pUz-GJcdRU|Arrays & For Loop|
|https://www.youtube.com/watch?v=IEqvmsqjpT0|Arrays related to Object|
|https://www.jetbrains.com/help/idea/2016.2/tutorial-debugging-your-first-java-application.html|How to debug using IntelliJ|
|https://youtu.be/Mr2mPu1tLhk?t=240|Adding a Maven Dependency (this is tip #8, tip #2 Comments at 1 min is also useful at this point)|


### Optional
| Link | Comment|
|:---- |:------ |
|http://commons.apache.org/proper/commons-lang/download_lang.cgi| What is "commons-lang"|
|https://www.jetbrains.com/help/idea/2016.2/configuring-project-and-global-libraries.html#lib_add_to_module_dependencies|How to add in a library|
|https://www.jetbrains.com/help/idea/2016.2/downloading-libraries-from-maven-repositories.html| Using Maven|
|https://www.youtube.com/watch?v=LOHBGyK3Hbs|Optional on LinkedLists|
|smartphone store|consider installing Sololearn Java Programming app|

## Assignment Review 

## Topics

### Add in a library
*There's a useful set of routines that exists outside of the main Java built-in statements which, as we are covering arrays, we'd like to loop in.*
- Why are there libraries
- How are they added so that IDEA knows about them
- How do you include them in a program; reference them in the code.

### Arrays
- overview
  - index and content
  - static vs dynamic
  - dimensioned (space allocated)
- initalise arrays
  - "new" 
  - redefine the values
  - declaration
  - initialise with values {"a","b"}
- loop through an array
- multi-dimensional arrays
- fill()
- Arrays.toString(*array variable*) __NOT__ *array variable*.toString as *Arrays* is a library function
- type in an array (i.e. Array&lt;type&gt;) 

*jagged arrays*

## Functions
- Purpose
- Return statement and value
- Input Parameters
- Scoping
  - re-use named variable
  - global variable
  - passing by reference vs value

## Main()
- Fixed invocation
- There can only be 1 per program
  - Identify which is the *entry* point
- How to read the parameter(s) passed

### Debugging - Introduction
- Setting a break point-  How to walk through the program
- Inspecting a variable

### Exceptions
- What can cause an exception
- Unhandled outcome



## Workshop/Practice 

### Challenge 1
### Challenge Final
- https://www.codewars.com/kata/descending-order/train/java

## Assignment
| Link | Comment|
|:---- |:------ |
|http://www.homeandlearn.co.uk/java/java_for_loops.html|Loop Exercises|
|http://blog.javafortesters.com/2016/07/how-to-debug-java-with-intellij.html|Describing how one uses the debugger in IntelliJ|

- Review loops, what causes them to terminate
- Stepping through programs; interogating variables.

