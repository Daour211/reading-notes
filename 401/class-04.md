## Objects & Class

**Object**

Object consist of state and behavior.

The states are saved in the fields to use. (variables)

The methods represent the behavior which will change and affect the state.

**Class**

Class like a blueprint from which object are created. It is an instance of the class object (main one)

## Java Classes:

### Declaring Class:

**This is class declaration:**
class MyClass {
// field, constructor, and
// method declarations
}

**For declaring a preceding class:**

class MyClass extends MySuperClass implements YourInterface {
// field, constructor, and
// method declarations
}

I can assign the class to one of two modifiers:

- **private**: does not permit other classes to access the class
- **public**: permit other classes to access the class

Class declarations can include these components in order:

1.  Modifiers <br>
2.  The class name<br>
3.  The name of the class's parent (superclass), if any, preceded by the keyword extends. A class can only extend (subclass) one parent.<br>
4.  A comma-separated list of interfaces implemented by the class, if any, preceded by the keyword implements. A class can implement more than one interface.<br>
5.  The class body

### Declaring variables:

Kinds of variables in class:

• Member variables in a class—these are called fields.<br>
• Variables in a method or block of code—these are called local variables.<br>
• Variables in method declarations—these are called parameters.

### Declaring methods:

method declarations have six components, in order:

1.  Modifiers.<br>
2.  The return type—the data type of the value returned by the method, or void if the method does not return a value.<br>
3.  The method name.<br>
4.  The parameter list in parenthesis—a comma-delimited list of input parameters, preceded by their data types, enclosed by parentheses, ().<br>
5.  An exception list<br>
6.  The method body

### Provide Constructor to Class

The class can have constructor to create objects from the class blueprint

I can pass information as arguments to constructor or method but I need to specify the type of data I am passing it

The user can pass an arbitrary value to a method by using construct called **varargs**. I use it when I don't know how many of a particular type of argument will be passed to the method.

**To use varargs, you follow the type of the last parameter by an ellipsis (three dots, ...), then a space, and the parameter name. The method can then be called with any number of that parameter.**

## Binary, Decimal and Hexadecimal Numbers:

**Decimals**

There is a decimal point which help us to know the position of a number.

**Bases**

Decimal Number System called Base 10 because based on the number 10. And the numbers “symbols” from 0-9.

**Resources**:

- [Objects & Class](https://docs.oracle.com/javase/tutorial/java/concepts/index.html)

- [Java Classes](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)

- [Binary, Decimal and Hexadecimal Numbers](https://www.mathsisfun.com/binary-decimal-hexadecimal.html)
