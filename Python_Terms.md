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
1.  **Object**
     * we can create many objects from a class. An object is also called an instance of a class and the process of creating this object is called instantiation.
      ![GitHub Logo](/images/object.png)
1.  **Static**
      * Static methods in Python are extremely similar to python class level methods, the difference being that a static method is bound to a class rather than the objects for that class.This means that a static method can be called without an object for that class. This also means that static methods cannot modify the state of an object as they are not bound to it. We created in claculator in miniproject 1 many static methods such as Addition etc.
        ![GitHub Logo](/images/static.png)
1.  **Property / Attribute**
      * In python, everything is an object. And every object has attributes and methods or functions. Attributes are described by data variables for example like name, age, height etc.
       ![GitHub Logo](/images/ww.png)
1.  **Method**
      * It's a function which is a member of a class: A method is a function that takes a class instance as its first parameter. Methods are members of classes.
        ![GitHub Logo](/images/method.png)
        


9. **Exception**

	An exception is an error that happens during execution of a program. When that error occurs, Python generate an exception that can be handled, which avoids your program to crash.


10. **Unit Test**

	Unit Testing is the first level of software testing where the smallest testable parts of a software are tested. This is used to validate that each unit of the software performs as designed. The unittest test framework is python's xUnit style framework.


11. **Constructor**

	A constructor is a special kind of method that Python calls when it instantiates an object using the definitions found in your class. Python relies on the constructor to perform tasks such as initializing (assigning values to) any instance variables that the object will need when it starts


12. **Factory**
	Factory method is a creational design pattern which solves the problem of creating product objects without specifying their concrete classes.

	Factory Method defines a method, which should be used for creating objects instead of direct constructor call (_new_ operator). Subclasses can override this method to change the class of objects that will be created.


13. **Decorator**

	A decorator is a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure. Decorators are usually called before the definition of a function you want to decorate.


14. **Extend Class**

	Python supports a feature called inheritance. By using inheritance, you can obtain the features you want from a parent class when creating a child class.

	Parent classes are normally supersets of something. For example, you might create a parent class named Car and then create child classes of various car types around it.

	In this case, you build a parent class named Animal and use it to define a child class named Chicken. Of course, you can easily add other child classes after you have Animal in place, such as a Gorilla class. However, for this example, you build just the one parent and one child class.

	The Animal class tracks three characteristics: Name, Age, and Type. A production application would probably track more characteristics, but these characteristics do everything needed for this example. The code also includes the required accessors for each of the characteristics. The __str__() method completes the picture by printing a simple message stating the animal characteristics.

	The Chicken class inherits from the Animal class. Notice the use of Animal in parentheses after the Chicken class name. This addition tells Python that Chicken is a kind of Animal, something that will inherit the characteristics of Animal.

	Someone might try something funny, such as setting her chicken up as a gorilla. With this in mind, the Chicken class also overrides the SetType() setter. If someone tries to change the Chicken type, that user gets a message rather than the attempted change. Normally, you handle this sort of problem by using an exception, but the message works better for this example by making the coding technique clearer.

	Finally, the Chicken class adds a new feature, MakeSound(). Whenever someone wants to hear the sound a chicken makes, he can call MakeSound() to at least see it printed on the screen.


15. **CSV Files**

	A **C**omma-**S**eparated **V**alues file is a delimited text file that uses a comma to separate values. A CSV file stores tabular data in plain text. Each line of the file is a data record. Each record consists of one or more fields, separated by commas



16. **Reading Files**

	When you’re working with Python, you don’t need to import a library in order to read and write files. It’s handled natively in the language, albeit in a unique manner.

