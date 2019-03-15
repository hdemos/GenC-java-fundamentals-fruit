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

###Method
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

lets call a method in our apple class that prints out how many days until the apple expires.
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


### Summary
Both __Fields__ and __Methods__ are used to make java objects so powerful and useful! 
Fields store object data and methods do actions to alter or use the object data. *An object is still a valid object even if it doesn't have any methods.*



Extra Resources 
https://medium.com/@madhupathy/a-beginners-guide-to-java-part-1-of-3-33edf47e47b4
