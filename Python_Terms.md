# SAMIA ALBLWI
# Python Terminology
1. **How Python uses Indentation to control Flow**
     * “control flow” in your code is to affect the order in which the code in your program is executed.
   Python’s syntax is quite flexible in terms of what it defines as a whitespace delimiter. Its rules are that:

    *One or more whitespace characters (spaces or tabs) is sufficient to serve as indentation.
    *A given indented block must use a uniform level of indentation. E.g. if the first line of an indented block has two leading spaces, all subsequent lines in that block must lead with exactly two white spaces.
    ![GitHub Logo](/images/Python_indentation.png)
1. **The DRY Principle: Don't Repeat Yourself**
      * DRY stand for "Don't Repeat Yourself," a basic principle of software development aimed at reducing repetition of information. The DRY principle is stated as, "Every piece of knowledge or logic must have a single, unambiguous representation within a system."
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

	 ![exception_handling](/images/exception_handling.png)

10. **Unit Test**

	Unit Testing is the first level of software testing where the smallest testable parts of a software are tested. This is used to validate that each unit of the software performs as designed. The unittest test framework is python's xUnit style framework.

	White Box Testing method is used for Unit testing

	**OOP concepts supported by unittest framework:**

	1. **test fixture:**
			A test fixture is used as a baseline for running tests to ensure that there is a fixed environment in which tests are run so that results are repeatable.

	2. **test case:**
			A test case is a set of conditions which is used to determine whether a system under test works correctly.

	3. **test suite:**
			Test suite is a collection of testcases that are used to test a software program to show that it has some specified set of behaviours by executing the aggregated tests together.

	4. **test runner:**
			A test runner is a component which set up the execution of tests and provides the outcome to the user.

	**Basic Test Structure**

		
	unittest defines tests by the following two ways :

			* Manage test “fixtures” using code.

			* test itself.

	![exception_handling](/images/unittest1.png)

	This is the basic test code using unittest framework, which is having a single test. This test() method will fail if TRUE is ever FALSE.

	**Running Tests**

	![exception_handling](/images/unittest2.png)

	The last block helps to run the test by running the file through the command line.

	![exception_handling](/images/unittest3.png)

	Here, in the output the “.” on the first line of output means that a test passed.
	
	“-v” option is added in the command line while running the tests to obtain more detailed test results.

	![exception_handling](/images/unittest3.png)

	**Outcomes Possible**

	There are three types of possible test outcomes :

		* OK – This means that all the tests are passed.

		* FAIL – This means that the test did not pass and an AssertionError exception is raised.

		* ERROR – This means that the test raises an exception other than AssertionError.

11. **Constructor**

	A constructor is a special kind of method that Python calls when it instantiates an object using the definitions found in your class. Python relies on the constructor to perform tasks such as initializing (assigning values to) any instance variables that the object will need when it starts.

	Constructors are generally used for instantiating an object.The task of constructors is to initialize(assign values) to the data members of the class when an object of class is created.In Python the __init__() method is called the constructor and is always called when an object is created.

	**Syntax of constructor declaration**

	![constructor](/images/constructor1.png)

	**Types of constructors**

	* **default constructor** :The default constructor is simple constructor which doesn’t accept any arguments.It’s definition has only one argument which is a reference to the instance being constructed.

	* **parameterized constructor** :constructor with parameters is known as parameterized constructor.The parameterized constructor take its first argument as a reference to the instance being constructed known as self and the rest of the arguments are provided by the programmer.

12. **Factory**
	Factory method is a creational design pattern which solves the problem of creating product objects without specifying their concrete classes.

	Factory Method defines a method, which should be used for creating objects instead of direct constructor call (_new_ operator). Subclasses can override this method to change the class of objects that will be created.

	The Factory module can be installed like any other pure Python module. Setuptools is supported but not required. You may also include the __Factory.py__ file directly in your project’s source tree, but you must retain the copyright notice and version and attribution information.

	![factory](/images/factory.png)


13. **Decorator**

	A decorator is a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure. Decorators are usually called before the definition of a function you want to decorate.

	Decorators are very powerful and useful tool in Python since it allows programmers to modify the behavior of function or class. Decorators allow us to wrap another function in order to extend the behavior of wrapped function, without permanently modifying it.

	In Decorators, functions are taken as the argument into another function and then called inside the wrapper function.

	**Syntax for Decorator**

	![decorator](/images/decorator.png)

	In the above code, gfg_decorator is a callable function, will add some code on the top of some another callable function, hello_decorator function and return the wrapper function.

14. **Extend Class**

	Python supports a feature called inheritance. By using inheritance, you can obtain the features you want from a parent class when creating a child class.

	Parent classes are normally supersets of something. For example, you might create a parent class named Car and then create child classes of various car types around it.

	![class_extension](/images/class_extension.png)

	In this case, you build a parent class named Animal and use it to define a child class named Chicken. Of course, you can easily add other child classes after you have Animal in place, such as a Gorilla class. However, for this example, you build just the one parent and one child class.

	The Animal class tracks three characteristics: Name, Age, and Type. A production application would probably track more characteristics, but these characteristics do everything needed for this example. The code also includes the required accessors for each of the characteristics. The __str__() method completes the picture by printing a simple message stating the animal characteristics.

	The Chicken class inherits from the Animal class. Notice the use of Animal in parentheses after the Chicken class name. This addition tells Python that Chicken is a kind of Animal, something that will inherit the characteristics of Animal.

	Someone might try something funny, such as setting her chicken up as a gorilla. With this in mind, the Chicken class also overrides the SetType() setter. If someone tries to change the Chicken type, that user gets a message rather than the attempted change. Normally, you handle this sort of problem by using an exception, but the message works better for this example by making the coding technique clearer.

	Finally, the Chicken class adds a new feature, MakeSound(). Whenever someone wants to hear the sound a chicken makes, he can call MakeSound() to at least see it printed on the screen.


15. **CSV Files**

	CSV (Comma Separated Values) is a simple file format used to store tabular data, such as a spreadsheet or database. A CSV file stores tabular data (numbers and text) in plain text. Each line of the file is a data record. Each record consists of one or more fields, separated by commas. The use of the comma as a field separator is the source of the name for this file format.

	![csv](/images/csv.png)

	For working CSV files in python, there is an inbuilt module called **csv.**
	
	16. **Reading Files**

	**Reading a CSV file**


	![csv](/images/csv1.png)

	The output of above program looks like this:

	![csv](/images/csv2.png)

	Let us try to understand this piece of code.

	![csv](/images/csvopen.png)

	Here, we first open the CSV file in READ mode. The file object is named as csvfile. The file object is converted to csv.reader object. We save the csv.reader object as **csvreader**.

	![csv](/images/csvfile.png)

	**csvreader** is an iterable object. Hence, .next() method returns the current row and advances the iterator to the next row. Since the first row of our csv file contains the headers (or field names), we save them in a list called **fields**.

	![csv](/images/csvrow.png)

	Now, we iterate through remaining rows using a for loop. Each row is appended to a list called **rows**. If you try to print each row, one can find that row is nothing but a list containing all the field values.

	![csv](/images/csvprint.png)

	**csvreader.line_num** is nothing but a counter which returns the number of rows which have been iterated.




