# GenC-java-fundamentals-fruit
Multiple Code Explorations for Java Fundamentals

## Exercise Objectives
* Create a proper variable name, leveraging the variable naming rules
* Use descriptive comments while creating the fruit class.
* Identify which words are java keywords

## Instructions
1. Fork this repository
2. Clone & open in your IDE
3. Work off the appropriate branch, 01-exercise branch is the first exercise

Use W3 Schools, Java Docs and your colleges to work through these exercises. Remember, it is important to code on your own computer as you will be tested on the concepts and use these or similar cocepts in your project. 

https://www.w3schools.com/java/default.asp

### Comments
Make sure to use descriptive comments in your code.
Java uses two forward slashes __//__ to note any comments in a .java file. 
A good programmer uses comments useful for those unfamiler with their code. Rather than commenting //refers to 2nd way to calculate x,
a better comment might be //this method calculates the area of a sphere . 

## Objects & Their Fields
When we say the “fields” of an object, we mean everything about that object. This is usually primitive types like integer, doubles, etc. An object can also have objects. 
These are sometimes referred to as __attributes__ or __member variables__.
For example, an apple object may contain fields like name, color and sweetness.
Then a fruit object might contain a field names apples that will store all the apples in an array.

### Accessing fields:
To access an object’s fields, you use the dot modifier ‘.’
So if you have an object called apple that contained the following fields:
```java
String name = honeycrisp;
String color;
int sweetnessScale;
```
To access the `name` field you would use 
```apple.name```
Which you can print like
```java
System.out.println(apple.name);
```
You can also store this in a string variable or manipulated it like any other string. 

```java
//This sets the variable myAppleName to honeycrisp
String myAppleName = apple.name;

//This changes the name field's value.
apple.name = Gala;
```




Extra Resources 
https://medium.com/@madhupathy/a-beginners-guide-to-java-part-1-of-3-33edf47e47b4
