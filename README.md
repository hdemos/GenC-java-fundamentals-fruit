# GenC-java-fundamentals-fruit
Multiple Code Explorations for Java Fundamentals

### Exercise Objectives
* Create a proper variable name, leveraging the variable naming rules
* Use descriptive comments while creating the fruit class.
* Identify which words are java keywords

### Instructions
1. Fork this repository
2. Clone & open in your IDE
3. Work off the appropriate branch, `exercises-fruit-objects` branch

Use W3 Schools, Java Docs and your colleges to work through these exercises. Remember, it is important to code on your own computer as you will be tested on the concepts solo and use these or similar concepts in your project. 

https://www.w3schools.com/java/default.asp

### Comments
Make sure to use descriptive comments in your code.
Java uses two forward slashes __//__ to note any comments in a .java file. 
A good programmer uses comments useful for those unfamiler with their code. Rather than commenting //refers to 2nd way to calculate x,
a better comment might be //this method calculates the area of a sphere . 


## Code Structure
Lets talk about the differences between a source flie, a class and a method. We will dive into detail after talking about how they are related.

A __source file__ is identified by its *.java* extenstion and it colds a single __class__ definiton. This class must be defined wihtin curly braces.

```java
public class Human{
  //this is a class
}
```


A __Class__ has variables and one or more __methods__, which are things that class does. This method must be declared inside a class (i.e. inside the curly braces).

```java
public class Human{
  void eat(){
  
  }

}
```

A __method__ has curly braces and inside these curly braces are where statements go like 'System.out.println("Human is eating");`



So, A class goes in a source file. A method goes in a class and statemends go in a method. 



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

### Method
In a class you might have seen notation like this

```java 
public void calcVal(){
  //code to calculate a value here
}
```


This called a __method__. 
*note: other languages use the term function*


Methods in java always belong to a specific object. 

#### Using Methods
To call a method, you also utizlie the dot modifier `.`

Lets call a method in our apple class that prints out how many days until the apple expires.
Here is the method
```java
//we have a variable named expiryDays
void getExpiryDays(){
    System.out.println(expiryDays);
}
```


Methods can also take in arguments. 


Lets say we want to set the Expiration Date. We would need to provide a value for the expiryDate to be set to. This is an argument.
```java
//here is the method definition
void setExpiryDays(int expiryDays){
  //code to set expiryDays
}
```
And if we wanted to call that function

```java
//if we had a function to set the expiryDays, this is what how you would call it
setExpiryDays(10);
```

##### Parameter vs Argument
These are often confused.
Checkout this resource to understand the difference.


[Parameter vs. Argument Medium Article](https://blog.kotlin-academy.com/programmer-dictionary-parameter-vs-argument-type-parameter-vs-type-argument-b965d2cc6929)


## Class vs Object
While they sound like they are refering to the same thing, these terms should not be used interchangably as they have distinct different meanings.

The easiest way to explain it is __objects__ are to __Classes__ like __variables__ are to __Data types__.

A __class__ is like a blueprint that defines things like variables and methods as we discussed earlier.


```java
//like we had our apple class
public class Apple {
  String name;
  ...
}
```

An __object__ is an instance of that class.


```java
Apple myApple = new Apple();
```


Here `myApple` is the object, or instance of the class Apple. 

Read [https://www.guru99.com/java-oops-class-objects.html] for more a walkthrough example on Classes vs Objects.




### Summary
Both __Fields__ and __Methods__ are used to make java objects so powerful and useful! 
Fields store data and methods do actions to alter or use that data. *A class is still a valid class even if it doesn't have any methods.*

A __class__ is a blueprint that defines how an object will behave and what data it will contain. An __object__ is a self-contained piece of code that consists of methods and variables. These are created when "newing up" an object with the `Class object = new Class();` statement. 


## Exercise 1
Make classes for a square, circle and triangle.
Each class should have a way to calculate the area and have name and color properties. 
The methods in the classes should print out the result of the calculation. 

Read *Chair Wars* from Head First Java



Extra Resources 
https://medium.com/@madhupathy/a-beginners-guide-to-java-part-1-of-3-33edf47e47b4

References: Head First Java
