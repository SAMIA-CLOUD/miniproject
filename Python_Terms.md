

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