# SAMIA ALBLWI
# Python Terminology
1. **How Python uses Indentation to control Flow**
     * “control flow” in your code is to affect the order in which the code in your program is executed.
   Python’s syntax is quite flexible in terms of what it defines as a whitespace delimiter. Its rules are that:

    *One or more whitespace characters (spaces or tabs) is sufficient to serve as indentation.
    *A given indented block must use a uniform level of indentation. E.g. if the first line of an indented block has two leading spaces, all subsequent lines in that block must lead with exactly two white spaces.
    ![GitHub Logo](/images/Python_indentation.png)
1. **The DRY Principle: Don't Repeat Yourself**
1. **Design Patterns from Gang of Four**
      * Everything starts with the Gang of Four (GOF). Do a quick online search if you are not familiar with the GOF.
      Design patterns are a common way of solving well known problems. 
      * Two main principles are in the bases of the design patterns defined by the GOF:
          * Program to an interface not an implementation.
          * Favor object composition over inheritance.
      * ![GitHub Logo](/images/GOF.png)
1. **Class**
      *  In object-oriented programming, a class is a blueprint for creating objects (a particular data structure), providing initial values for state (member variables or attributes), and implementations of behavior (member functions or methods). 
      *  ![GitHub Logo](/images/class.png)
      *  The image above shows how a Car object can be the template for many other Car instances. In the image, there are three instances: polo, mini, and beetle. Here, we will make a new class called Car, that will structure a Car object to contain information about the car’s model, the color, how many passengers it can hold, its speed, etc. A class can define types of operations, or methods, that can be performed on a Car object. For example, the Car class might specify an accelerate method, which would update the speed attribute of the car object. 
          ![GitHub Logo](/images/class_code.png)
      *  A class is a way of organizing information about a type of data so a programmer can reuse elements when making multiple instances of that data type—for example, if a programmer wanted to make three instances of Car, maybe a BMW, a Ferrari, and a Ford instance. The Car class would allow the programmer to store similar information that is unique to each car (they are different models, and maybe different colors, etc.) and associate the appropriate information with each car.
1. 