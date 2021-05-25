## Functional Programming Concepts

**Functions as first-class entities:**

The idea of functions as first-class entities is that functions are also treated as values and used as data. 
Functions as first-class entities can:
 -	refer to it from constants and variables
 - 	pass it as a parameter to other functions
 -	return it as result from other functions

**Higher-order functions**
 
 -	takes one or more functions as arguments, or
 -	returns a function as its result
 -	


Q1) What is functional programming? <br>
It is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

Q2) What is a pure function and how do we know if something is a pure function?<br>
It is a function that It returns the same result if given the same arguments & does not cause any observable side effects
The function is pure when:
  -	It returns the same result if given the same arguments (it is also referred as deterministic)

  -	Reading Files: If the function reads external files, it’s not a pure function — the file’s contents can change.

  -	Random number generation: Any function that relies on a random number generator cannot be pure.

  -	It does not cause any observable side effects; examples of observable side effects include modifying a global object or a parameter passed by reference.

Q3) What are the benefits of a pure function?<br>
The code’s definitely easier to test. So we can unit test pure functions with different contexts

Q4) What is immutability?<br>
Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created.

Q5) What is Referential transparency?<br>
It is term described for pure functions + immutable data. 


## Node JS Tutorial for Beginners #6 - Modules and require()


Q1) What is a module?
It is a JS file.

Q2) What does the word ‘require’ do?
It is used to get/pass the module we want by giving the path of the module as string parameters 

Q3) How do we bring another module into the file the we are working in?
By using the “require” method.

Q4) What do we have to do to make a module available?
We have to export the module and specify what we want to export.


**Resources:**
 - [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
 - [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)



